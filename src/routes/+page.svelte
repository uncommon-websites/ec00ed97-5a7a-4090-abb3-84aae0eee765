<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CenteredTextOnlyHero from "$lib/components/layout/hero-sections/CenteredTextOnlyHero.svelte";
	
	// Icons for Features
	import IconZap from "~icons/lucide/zap";
	import IconTrendingUp from "~icons/lucide/trending-up";
	import IconUsers from "~icons/lucide/users";
	import IconRefreshCw from "~icons/lucide/refresh-cw";
	import IconTarget from "~icons/lucide/target";
	import IconGlobe from "~icons/lucide/globe";
</script>

<CenteredTextOnlyHero
	title="Power that moves science forward"
	subtitle="Europa builds pulsed power platforms for civilian use—delivering fusion-grade conditions for industry, defense, space, and academia."
	imageSrc="/generated/image-a-wide-angle-documentary-style-photograp.webp"
/>
<LogoScroller 
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/airbus.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/lockheedmartin.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/thalesgroup.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/cern.ch/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	title="Technology advantages"
	subtitle="Breakthrough pulsed power systems that democratize access to fusion-grade experimental conditions"
	features={[
		{
			title: "Impedance-matched Marx generators",
			description: "Our proprietary Marx generator design delivers unmatched energy transfer efficiency through precision impedance matching. Revolutionary technology that sets new standards for pulsed power performance.",
			icon: IconZap
		},
		{
			title: "200× higher energy coupling efficiency",
			description: "Achieve fusion-grade conditions with dramatically superior efficiency compared to laser-driven systems. Game-changing performance that makes previously impossible experiments accessible.",
			icon: IconTrendingUp
		},
		{
			title: "Civilian access democratization", 
			description: "Break free from government facility bottlenecks with dedicated civilian pulsed power access. Open scheduling and transparent pricing unlock continuous research workflows.",
			icon: IconUsers
		},
		{
			title: "Repeatable experimental conditions",
			description: "Generate consistent, reproducible results with our stable pulsed power platform. Precision control enables systematic research programs and reliable data collection.",
			icon: IconRefreshCw
		},
		{
			title: "Multi-domain applications",
			description: "Serve space radiation testing, materials science, biomedical research, and academic programs from a single platform. One facility, unlimited experimental possibilities.",
			icon: IconTarget
		},
		{
			title: "European pulsed power leadership",
			description: "Establish Europe as a global leader in civilian pulsed power technology. Strategic independence from US facilities with world-class experimental capabilities.",
			icon: IconGlobe
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
