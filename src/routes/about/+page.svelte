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
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
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
<Culture {values} generating />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	generating
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
	generating
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
	generating
	title="Ready to collaborate?"
	subtitle="Let's create something amazing"
	description="Join the companies already leveraging our expertise to transform their digital presence and achieve their business goals."
/>
