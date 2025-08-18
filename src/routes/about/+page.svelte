<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Age expertise over generalization",
			description: "We believe kids and teens deserve therapists who truly understand their developmental stage. That's why we match families with specialists who only work with specific age ranges—so your child gets care that meets them exactly where they are."
		},
		{
			title: "Precision matching over trial and error",
			description: "No more guessing. Our smart intake process evaluates your child's needs and matches them with a licensed therapist who fits their age, condition, and schedule—often within 48 hours."
		},
		{
			title: "Urgency with quality",
			description: "We move fast, but never cut corners. Families shouldn't have to choose between speed and clinical excellence. We offer both—because when a child's mental health is at stake, delays aren't an option."
		}
	];
</script>

<SecondaryHero
	title="Therapy that grows with them"
	subtitle="Expert mental health support for every age"
	imageSrc="/generated/image-a-mother-and-her-young-daughter-are-sitt.webp"
	showCredibility={true}
	rating={4.94}
	improvementRate={89}
	familiesServed="100K+"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Every parent knows the feeling—seeing your child struggle and not knowing how to help. Whether it's anxiety, ADHD, low self-esteem, or something harder to name, the weight is heavy. You make calls, check referrals, unearth endless lists of wait times—only to find a six-week wait, maybe more. And all the while, your child still isn't sleeping well. Still avoiding school. Still unsure how to explain what's wrong. For families trying to find specialized mental health support for kids and teens, every day waiting feels like a day lost.",
		"Emora Health was created to change this reality. We built a platform that understands that a 7-year-old isn't just a \"small adult\"—they need care grounded in age-specific expertise. That's why we developed precision matching algorithms that connect families with therapists trained for their child's unique developmental stage. With less than a 10% therapist acceptance rate, every specialist we onboard meets the highest standards for clinical quality—and thanks to our partnerships with leading insurers, families can access care within 48 hours, not weeks, often for as little as $0–$30 per session.",
		"Today, over 1,000 families trust Emora with their child's mental health, and the results speak for themselves—89% see noticeable improvement in just five sessions. Our average therapist rating is 4.94 stars, and parents consistently tell us what a difference it makes to feel seen, supported, and guided. We're not just solving scheduling delays—we're transforming outcomes. Our mission is simple: give every child, teen, and young adult the tools to feel better, faster. Because kids deserve support that meets them where they are—and helps them grow."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our team."
	subtitle="Your partners in innovation."
	stakeholders={[
		{
			name: "Alex Morgan",
			position: "Founder & CEO",
			bio: "Started the company with a vision to transform the industry through innovative solutions.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Jamie Chen",
			position: "Chief Design Officer",
			bio: "Award-winning designer with a passion for creating intuitive and beautiful experiences.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Taylor Wright",
			position: "Head of Engineering",
			bio: "Technology enthusiast focused on building scalable systems that make a difference.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Help is just 48 hours away"
	subtitle="Get matched with the right therapist for your child"
	description="Join the 1,000+ families who trust Emora Health with their child's mental wellness. Skip the waitlists and connect with age-specialized therapists who truly understand your child's needs."
	imageSrc="/generated/image-a-parent-and-teenager-sitting-together-i.webp"
/>
