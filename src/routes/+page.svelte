<script>
    import Navbar from './components/Navbar.svelte';
    import Guidelines from './components/Guidelines.svelte';
  </script>
  
  <style>
    :global(body) {
      background-color: #282828;
      color: #f0f0f0;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
      margin: 0;
    }
    
    .container {
      display: flex;
      min-height: 100vh;
    }
    
    .navbar {
      width: 20%;
      min-height: 100vh;
    }
    
    .content {
      width: 80%;
      padding: 2rem;
    }
  </style>
  
  <div class="container">
    <div class="navbar">
      <Navbar />
    </div>
    <div class="content">
      <Guidelines />
    </div>
  </div>
  