<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Find the right therapist for your child"
	subtitle="Matched in 48 hours. Covered by insurance."
	imageSrc="/generated/image-a-cheerful-family-scene-featuring-a-pare.webp"
	centered={false}
/>
<LogoScroller 
	label="Trusted by families and schools nationwide"
	logoUrls={[
		'https://cdn.brandfetch.io/marriott.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/khanacademy.org/w/400/h/400/logo',
		'https://cdn.brandfetch.io/starbucks.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/target.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="How we help families"
	text="Emora Health connects your child or teen with a licensed, age-specific therapist in under 48 hours through our precision matching algorithm. No more six-week waitlists or uncertainty about finding the right specialist. We're covered by major insurers and focus exclusively on children, teens, and young adults ages 0-25."
/>

<Testimonials
	testimonials={[
		{
			name: "Carmen Rodriguez",
			position: "Mother of two",
			company: "Austin, TX",
			quote:
				"We went from a 6-week waitlist nightmare to having our therapist matched in just 24 hours. My 12-year-old connected with her specialist immediately, and with our insurance covering it, we're only paying $15 per session instead of the $300 we were quoted elsewhere.",
			image: "/generated/image-a-professional-headshot-of-a-confident-h.webp"
		},
		{
			name: "Marcus Thompson",
			position: "Father of three",
			company: "Denver, CO",
			quote:
				"After months of searching for someone who understood ADHD in teenagers, Emora matched us with an age-specific specialist who gets my 16-year-old. The quality ratings showed us exactly why she was perfect before we even started. No more guessing games with our child's mental health.",
			image: "/generated/image-a-professional-headshot-of-a-black-fathe.webp"
		},
		{
			name: "Jennifer Chen",
			position: "Working mother",
			company: "Seattle, WA",
			quote:
				"The evening appointments were a lifesaver for our busy family schedule. My 9-year-old daughter has grown so much in confidence after just 5 sessions. Knowing our therapist specializes in her exact age group gave us peace of mind that we were making the right investment in her future.",
			image: "/generated/image-a-professional-headshot-of-an-asian-amer.webp"
		}
	]}
/>

<Features
	title="Why families choose Emora"
	subtitle="Specialized care that transforms how children and teens experience mental health support"
	features={[
		{
			title: "Age-specialized therapists",
			description: "Our therapists specialize in specific developmental stages from early childhood through young adulthood. Each specialist understands the unique challenges and communication styles of their age group.",
			imageSrc: "/generated/image-a-diverse-group-of-mental-health-profess.webp"
		},
		{
			title: "48-hour matching guarantee",
			description: "Skip the 6+ week waitlists that plague traditional therapy. Our precision algorithms match your child with the perfect therapist within 48 hours.",
			imageSrc: "/generated/image-a-family-gathered-around-a-kitchen-table.webp"
		},
		{
			title: "Quality you can see",
			description: "Every therapist has a 4.9+ star rating with transparent reviews from families. Less than 10% of applicants meet our rigorous standards for clinical excellence.",
			imageSrc: "/generated/image-a-child-smiling-and-actively-participati.webp"
		},
		{
			title: "Insurance coverage included",
			description: "Most families pay just $0-$30 per session with major insurance providers. Say goodbye to $300+ therapy bills that drain your savings.",
			imageSrc: "/generated/image-a-parent-sitting-at-a-kitchen-table-surr.webp"
		},
		{
			title: "Precision matching algorithms",
			description: "Our technology analyzes 100+ factors to connect your child with therapists who specialize in their specific challenges, personality, and communication preferences.",
			imageSrc: "/generated/image-a-parent-and-child-sitting-comfortably-i.webp"
		},
		{
			title: "Proven outcomes for lasting growth",
			description: "89% of families see noticeable improvement within just 5 sessions. We focus on building lifelong resilience, not just temporary symptom relief.",
			imageSrc: "/generated/image-children-of-various-ages-playing-togethe.webp"
		}
	]}
/>
<AboutTeaser />
<CallToAction 
	title="Get matched with the right therapist in 48 hours"
	subtitle="Your child's mental health can't wait—neither should you"
	description="We connect you with a licensed, age-specialized therapist in under 48 hours, backed by a 4.94-star rating and covered by major insurance. Start your 3-minute matching quiz now and get care that works."
	imageSrc="/generated/image-a-joyful-parent-and-child-duo-beaming-wi.webp"
	callsToAction={[
		{
			href: "/get-started",
			label: "Start 3-minute quiz",
			variant: "primary"
		},
		{
			href: "/learn-more",
			label: "Learn more",
			variant: "secondary"
		}
	]}
/>
