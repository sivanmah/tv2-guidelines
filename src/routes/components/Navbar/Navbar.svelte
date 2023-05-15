<script>
	import { Hamburger } from 'svelte-hamburgers';


	let open = false;
	$: if (open) {
		console.log('open');
	}
	function scrollToSection(id) {
		const element = document.getElementById(id);
		element.scrollIntoView({ behavior: 'smooth' });
		open = false; // Close the menu when a link is clicked
	}

	function toggleMenu() {
		menuOpen = !menuOpen;
		console.log(menuOpen);
	}
</script>

<div class="hamburger-menu" on:click={toggleMenu}>
	<span />
	<span />
	<span />
</div>
<div>
	
<ul class:menu-open={open}>
	
	<li><a href="CO2">Data Carbon Calculator</a></li>	
	<li on:click={() => scrollToSection('planning')}>I. Planning</li>
	<li class="h3-title" on:click={() => scrollToSection('benchmark')}>A. Benchmark</li>
	<li class="h3-title" on:click={() => scrollToSection('theoretical-possibility')}>
		B. Theoretical Possibility
	</li>
	<li class="h3-title" on:click={() => scrollToSection('sustainability-budget')}>
		C. Sustainability Budget
	</li>
	<li class="h3-title" on:click={() => scrollToSection('stretch-goals')}>D. Stretch Goals</li>

	<li on:click={() => scrollToSection('design')}>II. Design and User Experience</li>
	<li class="h3-title" on:click={() => scrollToSection('yo-yo')}>A. Avoid Yo-Yo User Journeys</li>
	<li class="h3-title" on:click={() => scrollToSection('streamline-content')}>
		B. Streamline Content
	</li>
	<li class="h3-title" on:click={() => scrollToSection('dark-mode')}>C. Dark Mode</li>

	<li on:click={() => scrollToSection('content')}>III. Content Optimization</li>
	<li class="h3-title" on:click={() => scrollToSection('images')}>A. Images</li>
	<li class="h3-title" on:click={() => scrollToSection('typography')}>B. Typography</li>

	<li on:click={() => scrollToSection('power')}>IV. Power Consumption</li>
	<li class="h3-title" on:click={() => scrollToSection('color')}>A. Color</li>
	<li class="h3-title" on:click={() => scrollToSection('video')}>B. Video</li>
	<li class="h3-title" on:click={() => scrollToSection('gifs')}>C. GIFs</li>
	<li class="h3-title" on:click={() => scrollToSection('animations')}>D. Animations</li>

	<li on:click={() => scrollToSection('hosting')}>V. Hosting</li>
	<li class="h3-title" on:click={() => scrollToSection('green-host')}>A. Green Host</li>
	<li class="h3-title" on:click={() => scrollToSection('data-center')}>B. Data Center</li>
</ul>
</div>
<div class="hamburger-menu">
	<Hamburger bind:open --color="white" />
</div>

<style>
	@import './Navbar.css';
</style>
