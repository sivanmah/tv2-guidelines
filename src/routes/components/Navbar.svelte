<script>
    function scrollToSection(id) {
      const element = document.getElementById(id);
      element.scrollIntoView({ behavior: 'smooth' });
    }
  </script>
  
  <style>
ul {
    list-style-type: none;
    margin: 0;
    padding: 1rem;
    background-color: #1f1f1f;
    height: 100%;
  }

  li {
    cursor: pointer;
    padding: 0.5rem 0;
  }

  li:hover {
    color: #00aa00;
  }
</style>

<ul>
  <li on:click={() => scrollToSection('planning')}>I. Planning</li>
  <li on:click={() => scrollToSection('design')}>II. Design and User Experience</li>
  <li on:click={() => scrollToSection('content')}>III. Content Optimization</li>
  <li on:click={() => scrollToSection('power')}>IV. Power Consumption</li>
  <li on:click={() => scrollToSection('hosting')}>V. Hosting</li>
</ul>
  