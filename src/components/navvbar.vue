<template>
  <div>
    <nav class="nav-bar">
      <ul class="nav-bar-ul">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Learn More</a></li>
      </ul>
    </nav>
  </div>
</template>

<script setup></script>

<style>
.nav-bar {
  background-color: black;
  padding-top: 1px;
  padding-bottom: 1px;
  /* position: sticky; */
  top: 0;
  /* z-index: 5; */
}

.nav-bar-ul {
  width: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-evenly;
}

.nav-bar-ul li {
  list-style-type: none;
  text-align: center;
}

.nav-bar a {
  color: white;
  text-decoration: none;
  font-size: 1.2em;
}
</style>
