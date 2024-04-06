<template>
  <header class="header">
    <nav class="navigation">
      <a href="#home">Home</a>
      <a href="#Biodata">Biodata</a>
      <a href="#Skill">Skill</a>
      <a href="#Pengalaman">Pengalaman</a>
    </nav>
    <a href="#" class="more-link"></a>
  </header>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
body {
  margin: 0; /* Remove default margin */
  padding: 0; /* Remove default padding */
}

.header {
  position: fixed;
  top: 0;
  left: 0; /* Ensure the navbar starts from the left edge */
  width: 100%;
  background-color: #38220f; /* Dark background color */
  padding: 20px;
  display: flex;
  justify-content: space-between; /* Spread items evenly */
  align-items: center;
  z-index: 1000; /* Ensures the navbar stays on top of other content */
  box-sizing: border-box; /* Include padding in the width */
}

.navigation {
  display: flex;
  align-items: center;
}

.navigation a {
  color: #ece0d1;
  text-decoration: none;
  margin-right: 20px;
  font-family: 'Roboto', sans-serif; /* Use Roboto font */
}

.navigation a:hover {
  color: #dbc1ac; /* Orange color on hover */
  font-weight: bold; /* Bold font on hover */
}
</style>
