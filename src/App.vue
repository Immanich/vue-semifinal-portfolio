<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="container">
    <div class="sidebar">
      <div class="header">
        <img src="/public/botyok.jpg" alt="Profile Picture" style="width: 300px;">
        <h1 class="name"> Lord Immanuel Juanich</h1>
        <h3 class="subtitle">BSIT - 3</h3>
      </div>
      <iframe width="300" height="315" src="https://www.youtube.com/embed/X1Cs2oz1LFY" title="Oddly Satisfying Video with Calming Deep Sleep Music _ Stress Relief &amp; Meditation #S54" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
      <nav class="navigation">
        <ul>
          
          <li>
            <button class="button py-4 px-8 text-white bg-black-200 hover:bg-black-300 duration-300 shadow-none">EMAIL ME</button>
          </li>
        </ul>
      </nav>
    </div>
    <div class="content">
      <RouterView />
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Baloo+2:wght@400;700&display=swap');

.button {
  margin-left: 5rem;
  padding: 1.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 300ms;
  font-size: medium;
  font-weight: bold;
  background-color: #d2d2d2;
  border-radius: 5px;
  cursor: pointer;
}

.button:hover {
  background-color: #bbbbbb;
}

body {
  margin: 0;
  padding: 0;
}

.container {
  margin: 0;
  display: flex;
  font-family: cursive;
  /* background: linear-gradient(to right, #ffffff, #656a6c); Gradient background */
  background-color: #fff;
}

.sidebar {
  width: 300px;
  background: #656a6c; 
  color: #6c6d6f;
  padding: 1rem;
}

.header {
  text-align: center;
}

.profile-picture {
  width: 50%;
  height: auto;
  margin-bottom: 20px;
  border-radius: 20%; 
  overflow: hidden; 
  transition: transform 0.2s ease, opacity 0.3s ease; 
}

/* .profile-picture:hover {
  transform: scale(1.1); 
  opacity: 0.8; 
} */

.name {
  margin-bottom: 0.2rem;
  font-size: 2em;
  color: #e6f2ff;
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

.subtitle {
  font-size: 1.8em;
  color: #6ec5ff; 
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

.navigation {
  margin-top: 20px;
}

.navigation ul {
  list-style-type: none;
  padding: 0;
}

.navigation li {
  margin-bottom: 10px;
}

.navigation a {
  text-decoration: none;
  color: #2c3e50; 
  display: flex;
  align-items: center;
  font-size: 1.1em;
  transition: transform 0.2s ease, background-color 0.3s ease, color 0.3s ease;
  border-radius: 5px;
  padding: 10px;
}

.navigation i {
  margin-right: 10px;
}

.navigation a:hover {
  background-color: #ecf0f1; 
  color: #e74c3c; 
  transform: translateX(5px); 
}

.content {
  flex: 1;
  padding: 20px;
}

.content h2 {
  color: #2c3e50;
  font-size: 1.8em;
  margin-bottom: 20px;
}

.content p {
  color: #555;
  line-height: 1.6;
  font-size: 1.1em;
}

.email-box {
  background-color: #0c0d0f;
  padding: 10px;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}

.email-box:hover {
  background-color: #2980b9;
}
</style>
