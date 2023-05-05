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
<section id="planning">
    <h2>I. Planning</h2>
    <h3 id="benchmark">A. Benchmark</h3>
    <p>Assess the sustainability of your website and compare it with competitor sites.</p>
    <h3 id="theoretical-possibility">B. Theoretical Possibility</h3>
    <p>Determine the best possible metrics for your website under ideal conditions.</p>
    <h3 id="sustainability-budget">C. Sustainability Budget</h3>
    <p>Set sustainability goals that are achievable and at least on par with industry standards. If there's potential for significant improvement, aim for a higher sustainability budget.</p>
    <h3 id="stretch-goals">D. Stretch Goals</h3>
    <p>Establish ambitious targets to pursue once the sustainability budget goals are met.</p>
  </section>
  
  <section id="design">
    <h2>II. Design and User Experience</h2>
    <h3 id="yo-yo">A. Avoid Yo-Yo User Journeys</h3>
    <p>Prevent users from frequently navigating in and out of pages. For example, eliminate the need to return to the homepage to access different pages.</p>
    <h3 id="streamline-content">B. Streamline Content</h3>
    <p>Reevaluate the necessity of your website's pages and content. Less is more for sustainability.</p>
    <h3 id="dark-mode">C. Dark Mode</h3>
    <p>Implement an automatic dark mode or adopt a dark mode-first approach for OLED screens.</p>
  </section>
  
  <section id="content">
    <h2>III. Content Optimization</h2>
    <h3 id="images">A. Images</h3>
    <p>1. File Type: Use WEBP instead of JPEG for 30% smaller file size. Use PNG or GIF for images with few block colors, like icons.</p>
    <p>2. Optimization: Utilize tools like Shortpixel, TinyPNG, or ImageAlpha to reduce image file sizes.</p>
    <p>3. Responsive Images: Employ "srcset" and "sizes" attributes in HTML "picture" elements to display images based on screen size.</p>
    <p>4. Additional Techniques: Implement blurring, CSS monochrome or grayscale, and SVG optimization to further reduce file size.</p>
    <p>5. Image Spacing: Reduce image width and height to decrease file size and enhance impact.</p>
    <h3 id="typography">B. Typography</h3>
    <p>1. System Fonts: Use pre-installed system fonts to avoid data transfer.</p>
    <p>2. Font Hosting: Host font files on your server instead of using font services to reduce server requests.</p>
    <p>3. Font Files: Remove unneeded files and use variable fonts for multiple font styles. Convert files to WOFF2 format.</p>
    <p>4. Optimization: Use tools like Fontdrop and Everything Fonts to remove unused characters, subject to foundry license terms.</p>
  </section>
  
  <section id="power">
    <h2>IV. Power Consumption</h2>
    <h3 id="color">A. Color</h3>
    <p>Dark colors use less power on OLED screens. Optimize color usage with tools like Codepen.</p>
    <h3 id="video">B. Video</h3>
    <p>Minimize video usage and autoplay. Opt for images, text, or interactive CSS animations when possible.</p>
    <h3 id="gifs">C. GIFs</h3>
    <p>Replace GIF animations with more efficient WEBP files.</p>
    <h3 id="animations">D. Animations</h3>
    <p>Limit front-end animations to reduce CPU usage.</p>
  </section>

  <section id="hosting">
    <h2>V. Hosting</h2>
    <h3 id="green-host">A. Green Host</h3>
    <p>Ensure your website is hosted on a data center powered by green energy.</p>
    <h3 id="data-center">B. Data Center</h3>
    <p>Select a data center close to your core user base to reduce emissions and latency.</p>
  </section>