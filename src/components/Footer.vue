<template>
  <div>
    <footer class="footer">
      <ul>
        <li><a href="#" target="_blank">Twitter</a></li>
        <li><a href="#" target="_blank">Facebook</a></li>
        <li><a href="#" target="_blank">Instagram</a></li>
      </ul>
    </footer>
  </div>
</template>

<script setup></script>

<style>
.footer {
  font-size: 1.2em;
  text-align: center;
  background-color: black;
  margin-top: 100px;
}

.footer a {
  color: whitesmoke;
  text-decoration: none;
  padding-top: 1px;
  padding-bottom: 1px;
}

.footer ul {
  list-style: none;
  width: 100%;
  display: flex;
  justify-content: space-evenly;
}
</style>
