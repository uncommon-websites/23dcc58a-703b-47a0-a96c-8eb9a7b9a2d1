<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	
	// Icons
	import IconStar from "~icons/lucide/star";
	import IconCheckCircle from "~icons/lucide/check-circle";
	import IconUsers from "~icons/lucide/users";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		showCredibility = false,
		rating = null,
		improvementRate = null,
		familiesServed = null,
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		showCredibility?: boolean;
		rating?: number | null;
		improvementRate?: number | null;
		familiesServed?: string | null;
		[key: string]: any;
	} = $props();
</script>

<header class="border-b border-gray-100 dark:border-gray-900" {...rest}>
	<div class="text-title3 section-px section-py container mx-auto grid gap-16 gap-y-0">
		<div class="space-y-8">
			<SectionHeader {title} {subtitle} size="lg" />
			
			{#if showCredibility && (rating || improvementRate || familiesServed)}
				<div class="flex flex-wrap gap-8 justify-center md:justify-start">
					{#if rating}
						<div class="flex items-center gap-2 bg-primary-50 text-primary-800 px-4 py-2 rounded-full">
							<IconStar class="w-5 h-5 fill-current" />
							<span class="text-body font-medium">{rating} stars from 1,000+ families</span>
						</div>
					{/if}
					
					{#if improvementRate}
						<div class="flex items-center gap-2 bg-secondary-50 text-secondary-800 px-4 py-2 rounded-full">
							<IconCheckCircle class="w-5 h-5" />
							<span class="text-body font-medium">{improvementRate}% improvement in 5 sessions</span>
						</div>
					{/if}
					
					{#if familiesServed}
						<div class="flex items-center gap-2 bg-accent text-accent-foreground px-4 py-2 rounded-full">
							<IconUsers class="w-5 h-5" />
							<span class="text-body font-medium">{familiesServed} families served</span>
						</div>
					{/if}
				</div>
			{/if}
		</div>
		
		<div class="aspect-video overflow-clip rounded-xl bg-muted">
			<img
				class="h-full w-full object-cover"
				src={imageSrc}
				alt="Our dedicated team of mental health professionals working together"
			/>
		</div>
	</div>
</header>
