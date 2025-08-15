<!--
@component AboutTeaser
A minimalist teaser for the about page.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Dr. Sarah Chen",
		role: "Founder & CEO",
		image: "/generated/image-a-professional-female-founder-in-her-mid.webp"
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-3xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"I couldn't find a therapist who truly got kids. So we built the one I wish I had when my son needed help."`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="grid items-center gap-6 dark:border-gray-800">
				<div class="flex items-center justify-center gap-6">
					<img
						src={teamMember.image}
						alt={teamMember.name}
						class="size-16 rounded-full object-cover"
					/>
					<div class="flex flex-col items-start">
						<div class="text-callout font-semibold">{teamMember.name}</div>
						<div class="text-caption text-emphasis-low mb-2">{teamMember.role}</div>
						<div class="text-caption text-emphasis-medium">
							Former pediatric psychologist turned entrepreneur
						</div>
					</div>
				</div>
				
				<div class="flex justify-center">
					<Button href="/about" variant="primary" size="md" class="rounded-full">
						Read her story
					</Button>
				</div>
			</div>
		</div>
	</div>
</section>
