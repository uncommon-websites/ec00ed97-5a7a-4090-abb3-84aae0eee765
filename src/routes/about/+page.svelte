<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Access democratization",
			description: "Opening Europe's first commercially accessible pulsed power facility, transforming episodic research into continuous innovation."
		},
		{
			title: "Technical excellence",
			description: "Achieving 200× higher energy coupling efficiency through impedance-matched Marx generators and magnetized liner inertial fusion."
		},
		{
			title: "Scientific acceleration",
			description: "Enabling breakthrough discoveries in space technology, materials science, and fusion energy by providing repeatable access to extreme conditions."
		}
	];
</script>

<SecondaryHero
	title="Powering fusion. Opening access."
	subtitle="Pulsed energy for science, space, and the grid"
	imageSrc="/generated/image-a-research-team-of-diverse-scientists-an.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"For too long, groundbreaking research in space technology, materials science, and fusion energy has been bottlenecked by limited access to the most advanced pulsed power facilities. While companies like Airbus, Thales Alenia, and research institutions across Europe have pressing needs to test electronics under extreme radiation, study materials at megabar pressures, and validate fusion concepts, they face years-long waiting lists at government facilities or settle for inadequate approximations that don't capture real-world conditions.",
		"Europa Energy was founded to democratize access to this critical technology through our impedance-matched Marx generators and magnetized liner inertial fusion approach. By achieving 200× higher energy coupling efficiency than laser-driven systems at one-tenth the capital cost, we're building Europe's first commercially accessible pulsed power facility. Our journey from proof-of-concept experiments to facility-scale operations focuses on creating repeatable, bookable access to the extreme conditions that drive innovation.",
		"Our vision extends beyond access – we're pioneering the path to fusion energy on the grid while building a thriving ecosystem of research and development. Every experiment run at our facility advances not just individual projects, but the entire field of high-energy density physics. By making continuous rather than episodic research possible, we're accelerating the pace of discovery that will define the next generation of space exploration, materials engineering, and clean energy solutions."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our founder."
	subtitle="Leading Europe's pulsed power revolution."
	stakeholders={[
		{
			name: "Nantas Nardelli",
			position: "Founder & CEO",
			bio: "Former head of ML at Pacific Fusion, AI lead at Carbon Re, and deep learning researcher with extensive experience in plasma physics modeling, target design, and fusion energy systems.",
			image: "/generated/image-professional-headshot-of-a-male-ceo-in-a.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to partner with us?"
	subtitle="Accelerate your research capabilities"
	description="Join the space agencies, research institutions, and technology companies already leveraging our pulsed power facility to advance their most ambitious projects."
	imageSrc="/generated/image-a-professional-research-scientist-deeply.webp"
/>
