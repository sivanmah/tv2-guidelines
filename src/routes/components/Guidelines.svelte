<script>
	let activeSections = [];

	function toggleSection(index) {
		const isActive = activeSections.includes(index);
		if (isActive) {
			activeSections = activeSections.filter((x) => x !== index);
		} else {
			activeSections = [...activeSections, index];
		}
		console.log(activeSections);
	}
</script>

<section id="planning">
	<h2>I. Planning</h2>
	<h3 id="benchmark">A. Benchmark</h3>
	<p on:click={() => toggleSection(0)} class:active={activeSections.includes(0)}>
		<span class={activeSections.includes(0) ? 'arrow down' : 'arrow up'} />Assess the sustainability
		of your website and compare it with competitor sites.
	</p>
	<div class={activeSections.includes(0) ? 'info' : 'hidden'}>
		<p>
			There are different ways of measuring sustainability. You can use online tools such as
			https://www.websitecarbon.com/ to measure your own website as well as competitors. You can
			also use Google Lighthouse to measure the performance of these websites, as there is often a
			correlation between a website's performance and its sustainability.
		</p>
		<p>
			Many cloud services such as Google Cloud have dashboard that are specifically designed to help
			developers with measuring their sustainability.
		</p>
	</div>
	<h3 id="theoretical-possibility">B. Theoretical Possibility</h3>
	<p on:click={() => toggleSection(1)} class:active={activeSections.includes(1)}>
		<span class={activeSections.includes(1) ? 'arrow down' : 'arrow up'} />Determine the
		theoretically best possible sustainability results for your website.
	</p>
	<div class={activeSections.includes(1) ? 'info' : 'hidden'}>
		<p>
			The theoretical best possible res are measurements of sustainability that are what seem to be
			the best-case scenario for your website, under the best possible conditions.
		</p>
		<p>
			The benchmark from the previous point shows you what's already done, but it doesn't tell you
			how much better you can do. Note that the theoretical best possible results often are not
			achievable in practice.
		</p>
		<p>
			For example, your website might get the best possible page weight by not using a custom font,
			but you might not want to sacrifice the design of your website for this.
		</p>
	</div>
	<h3 id="sustainability-budget">C. Sustainability Budget</h3>
	<p on:click={() => toggleSection(2)} class:active={activeSections.includes(2)}>
		<span class={activeSections.includes(2) ? 'arrow down' : 'arrow up'} />Set sustainability goals
		that are achievable and at least on par with industry standards. If there's potential for
		significant improvement, aim for a higher sustainability budget.
	</p>
	<div class={activeSections.includes(2) ? 'info' : 'hidden'}>
		<p>
			This describes what metrics you want to be displayed for your website the next time you run
			benchmarks on it. Your sustainability should be set to be at least as good as the best in the
			industry, and ideally with the ability to improve further. If there's a lot of room between
			best in industry and theoretically best, then you should consider improving much further. Most
			importantly every budget for each metric should be something you're confident you can achieve.
		</p>
	</div>
	<h3 id="stretch-goals">D. Stretch Goals</h3>
	<p on:click={() => toggleSection(3)} class:active={activeSections.includes(30)}>
		<span class={activeSections.includes(3) ? 'arrow down' : 'arrow up'} />Establish ambitious
		targets to pursue once the sustainability budget goals are met.
	</p>
	<div class={activeSections.includes(3) ? 'info' : 'hidden'}>
		It can be worth it to set stretch goals that are more ambitious than your sustainability budget,
		after you have fullfilled that budget. Set goals that are ambitious, but still achievable.
	</div>
</section>

<section id="design">
	<h2>II. Design and User Experience</h2>
	<h3 id="yo-yo">A. Avoid Yo-Yo User Journeys</h3>
	<p on:click={() => toggleSection(4)} class:active={activeSections.includes(4)}>
		<span class={activeSections.includes(4) ? 'arrow down' : 'arrow up'} />Prevent design that makes
		users repeatedly go in and out of a page to effectively use your website.
	</p>
	<div class={activeSections.includes(4) ? 'info' : 'hidden'}>
		Common examples of this is users going back to the homepage to be able to navigate to a
		different page, or making users go the shopping cart page to view what is inside their cart.
		This can be solved by adding a navigation bar to all pages, and adding letting you view your
		cart from any page by hovering over a cart icon.
	</div>

	<h3 id="streamline-content">B. Streamline Content</h3>
	<p on:click={() => toggleSection(5)} class:active={activeSections.includes(4)}>
		<span class={activeSections.includes(5) ? 'arrow down' : 'arrow up'} />
		Reevaluate the necessity of your website's pages and content. Less is more for sustainability.
	</p>
	<div class={activeSections.includes(5) ? 'info' : 'hidden'}>
		In-depth explanation and examples for section I.A. Benchmark...
	</div>
	<h3 id="dark-mode">C. Dark Mode</h3>
	<p on:click={() => toggleSection(6)} class:active={activeSections.includes(6)}>
		<span class={activeSections.includes(6) ? 'arrow down' : 'arrow up'} />Implement a dark mode
		palette that automatically activates for users that have a dark mode preference.
	</p>
	<div class={activeSections.includes(6) ? 'info' : 'hidden'}>
		Also consider using a dark mode first approach, more than 1 billion smartphones use OLED
		technology, which with dark mode could reduce their power draw by up to 47%.
	</div>
</section>

<section id="content">
	<h2>III. Content Optimization</h2>
	<h3 id="images">A. Images</h3>
	<p on:click={() => toggleSection(7)} class:active={activeSections.includes(7)}>
		<span class={activeSections.includes(7) ? 'arrow down' : 'arrow up'} />1. File Type: Use WEBP
		instead of JPEG for 30% smaller file size. Use PNG or GIF for images with few block colors, like
		icons.
	</p>
	<div class={activeSections.includes(7) ? 'info' : 'hidden'}>
		<p>In-depth explanation and examples for section I.A. Benchmark...</p>
	</div>

	<p on:click={() => toggleSection(21)} class:active={activeSections.includes(21)}>
		<span class={activeSections.includes(21) ? 'arrow down' : 'arrow up'} />
		2. Optimization: Utilize tools like Shortpixel, TinyPNG, or ImageAlpha to reduce image file sizes.
	</p>
	<div class={activeSections.includes(21) ? 'info' : 'hidden'}>
		<p>Icon and logo PNGs can be optimized with ImageAlpha to compress from 24-bit to PNG-8.</p>
	</div>
	<p on:click={() => toggleSection(8)} class:active={activeSections.includes(8)}>
		<span class={activeSections.includes(8) ? 'arrow down' : 'arrow up'} />3. Responsive Images:
		Employ "srcset" and "sizes" attributes in HTML "picture" elements to display images based on
		screen size.
	</p>
	<div class={activeSections.includes(8) ? 'info' : 'hidden'}>
		<p>
			This allows you to display different images based on the needs of the user. So that for
			example a mobile user will not be downloading a large image that is only needed for desktop
			users.
		</p>
	</div>

	<p on:click={() => toggleSection(9)} class:active={activeSections.includes(9)}>
		<span class={activeSections.includes(9) ? 'arrow down' : 'arrow up'} />4. Additional Techniques:
		Implement blurring, monochrome or grayscale, and SVG optimization to further reduce file of
		images size.
	</p>
	<div class={activeSections.includes(9) ? 'info' : 'hidden'}>
		<p>
			Blur reduces an image’s file size. Use shallow depth of field for photographs, or blur the
			edges, or around the main object of the photo. This way you reduce file size to nearly half.
			Use CSS monochrome or grayscale on an image to successfully reduce the file size.
		</p>

		<p>
			Replace images with SVGs whenever possible. Edit the SVG in Adobe Illustrator and remove
			unused groups, layers and unnecessary anchor points. Then use ImageOptim to further optimize
			the SVG. This results in an 85% smaller SVG file, without any visual changes.
		</p>
	</div>

	<p on:click={() => toggleSection(10)} class:active={activeSections.includes(10)}>
		<span class={activeSections.includes(10) ? 'arrow down' : 'arrow up'} />5. Image Spacing: Reduce
		image width and height to decrease file.
	</p>
	<div class={activeSections.includes(10) ? 'info' : 'hidden'}>
		<p>
			More space around images will reduce the file size while also making the images more
			impactful.
		</p>
	</div>

	<h3 id="typography">B. Typography</h3>
	<p on:click={() => toggleSection(11)} class:active={activeSections.includes(11)}>
		<span class={activeSections.includes(11) ? 'arrow down' : 'arrow up'} />1. System Fonts: Use
		pre-installed system fonts to avoid data transfer.
	</p>
	<div class={activeSections.includes(11) ? 'info' : 'hidden'}>
		<p>
			System fonts are pre-installed on most systems, and therefore always the most efficient since
			they require no additional data transfer.
		</p>
	</div>

	<p on:click={() => toggleSection(12)} class:active={activeSections.includes(12)}>
		<span class={activeSections.includes(12) ? 'arrow down' : 'arrow up'} />2. Font Hosting: Host
		font files on your server instead of using font services to reduce server requests.
	</p>
	<div class={activeSections.includes(12) ? 'info' : 'hidden'}>
		<p>
			Font services like Google Fonts and Adobe Fonts are convenient, but they require additional
			server requests, which leads to more data transfer. Hosting font files on your server will
			reduce server requests.
		</p>
	</div>

	<p on:click={() => toggleSection(13)} class:active={activeSections.includes(13)}>
		<span class={activeSections.includes(13) ? 'arrow down' : 'arrow up'} />3. Font Files: Remove
		unneeded files and use variable fonts for multiple font styles. Convert files to WOFF2 format.
	</p>
	<div class={activeSections.includes(13) ? 'info' : 'hidden'}>
		In-depth explanation and examples for section I.A. Benchmark...
	</div>

	<p on:click={() => toggleSection(14)} class:active={activeSections.includes(14)}>
		<span class={activeSections.includes(14) ? 'arrow down' : 'arrow up'} />4. Optimization: Use
		tools to to remove unused characters, subject to foundry license terms.
	</p>
	<div class={activeSections.includes(14) ? 'info' : 'hidden'}>
		<p>
			Fonts will often include characters for languages you may not be in need of, as well as other
			unneeded characters. Use tools such as https://fontdrop.info along with
			https://everythingfonts.com/subsetter to see all the characters that are included in your font
			file, then remove all the characters that are not necessary.
		</p>
		<p class="bold">
			NB! Only do this if the foundry’s license terms allow for web use and optimization.
		</p>
	</div>
</section>

<section id="power">
	<h2>IV. Power Consumption</h2>
	<h3 id="color">A. Color</h3>
	<p on:click={() => toggleSection(15)} class:active={activeSections.includes(15)}>
		<span class={activeSections.includes(15) ? 'arrow down' : 'arrow up'} />Dark colors use less
		power on OLED screens. Blue uses less power than green and red.
	</p>
	<div class={activeSections.includes(15) ? 'info' : 'hidden'}>
		Blue pixels use 25% more power than green and red pixels. Black pixels are the most efficient
		for OLED screens, since the diodes will be turned off. Dark colours in general use less power,
		so use them as much as possible. You can use https://codepen.io/stoumann/full/vYgzpNp to see how
		much energy an image will use, based on its colours.
	</div>

	<h3 id="video">B. Video</h3>
	<p on:click={() => toggleSection(16)} class:active={activeSections.includes(16)}>
		<span class={activeSections.includes(16) ? 'arrow down' : 'arrow up'} />Minimize video usage and
		autoplay. Opt for images, text, or interactive CSS animations when possible.
	</p>
	<div class={activeSections.includes(16) ? 'info' : 'hidden'}>
		<p>
			Users don’t always want videos. They use a lot of power and data from the user. Additionally
			it is often not convenient for users to watch videos, especially if they are in a public
			space. Replace videos with Images, text, or interactive CSS animations whenever possible.
		</p>
		<p>
			If you need to use videos, make sure they are not set to autoplay. Autoplaying videos are bad
			for sustainability and accessibility.
		</p>
	</div>

	<h3 id="gifs">C. GIFs</h3>
	<p on:click={() => toggleSection(17)} class:active={activeSections.includes(17)}>
		<span class={activeSections.includes(17) ? 'arrow down' : 'arrow up'} />Replace GIF animations
		with more efficient WEBP files.
	</p>
	<div class={activeSections.includes(17) ? 'info' : 'hidden'}>
		<p>
			GIFs are a very inefficient file format, and should be avoided whenever possible. Use WEBP
			files instead, which are much more efficient.
		</p>
	</div>

	<h3 id="animations">D. Animations</h3>
	<p on:click={() => toggleSection(18)} class:active={activeSections.includes(18)}>
		<span class={activeSections.includes(18) ? 'arrow down' : 'arrow up'} />Limit front-end
		animations to reduce CPU usage.
	</p>
	<div class={activeSections.includes(18) ? 'info' : 'hidden'}>
		<p>
			Front-end animations can significantly increase CPU usage on the user’s device. Have just
			enough animations to make the website feel nice to use.
		</p>
	</div>
</section>

<section id="hosting">
	<h2>V. Hosting</h2>
	<h3 id="green-host">A. Green Host</h3>
	<p on:click={() => toggleSection(19)} class:active={activeSections.includes(19)}>
		<span class={activeSections.includes(19) ? 'arrow down' : 'arrow up'} />Ensure your website is
		hosted on a data center powered by green energy.
	</p>
	<div class={activeSections.includes(19) ? 'info' : 'hidden'}>
		<p>
			There are many hosting providers that use green energy. Some of them are listed here:
			<a href="https://www.thegreenwebfoundation.org/directory/"
				>https://www.thegreenwebfoundation.org/directory/</a
			>
		</p>
	</div>

	<h3 id="data-center">B. Data Center</h3>
	<p on:click={() => toggleSection(20)} class:active={activeSections.includes(20)}>
		<span class={activeSections.includes(20) ? 'arrow down' : 'arrow up'} />Select a data center
		close to your core user base to reduce emissions and latency.
	</p>
	<div class={activeSections.includes(20) ? 'info' : 'hidden'}>
		<p>
			The farther the data has to travel to reach the user, the more emissions are produced from
			telecom networks. Therefore it is important to select a data center that is close to your core
			user base.
		</p>
	</div>
</section>

<style>
	h2 {
		margin-top: 2rem;
		margin-bottom: 1rem;
	}

	h3 {
		margin-top: 1.5rem;
		margin-bottom: 0.5rem;
	}

	@media (max-width: 1024px) {
		h2 {
			font-size: 1.5rem;
		}

		h3 {
			font-size: 1.25rem;
		}
	}

	.hidden {
		display: none;
	}

	.info {
		background-color: #333;
		color: #fff;
		padding: 1rem;
		border-radius: 0.5rem;
		margin: 0.5rem 0;
	}

	.arrow {
		border: solid;
		border-width: 0 0.1rem 0.1rem 0;
		display: inline-block;
		padding: 0.25rem;
		margin-right: 0.5rem;
	}

	.down {
		transform: rotate(45deg);
		-webkit-transform: rotate(45deg);
	}

	.up {
		transform: rotate(-135deg);
		-webkit-transform: rotate(-135deg);
	}

	h3 ~ p {
		cursor: pointer;
		margin-bottom: 0.5rem;
	}

	h3 ~ p:hover {
		color: #00aa00;
	}

	.bold {
		font-weight: bold;
	}

	@media (max-width: 768px) {
		h2 {
			font-size: 1.25rem;
			margin-top: 1.5rem;
		}

		h3 {
			font-size: 1.125rem;
			margin-top: 1.25rem;
		}
	}

	@media (max-width: 480px) {
		h2 {
			font-size: 1rem;
			margin-top: 1rem;
		}

		h3 {
			font-size: 0.875rem;
			margin-top: 1rem;
		}
	}
</style>
