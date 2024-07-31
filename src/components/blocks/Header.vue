<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="header">
      <div class="left">
        <RouterLink to="/">
          <h1 class="title"><b style="font-weight: bold">Streamy</b></h1>
        </RouterLink>
      </div>
      <div class="right">
        <a
          href="https://dash.streamy.gg"
          target="_blank"
          rel="noopener noreferrer"
        >
          <h1 class="dashboard">
            <font-awesome-icon :icon="['fa', 'gear']" /> Dashboard
          </h1>
        </a>
      </div>
    </div>
  </header>
</template>

<style lang="scss">
.header {
  display: flex;
  color: white;
  justify-content: space-between;
  align-items: center;
  padding: 10px 25px;
  box-shadow: 0 4px 4px 0 rgba(0, 0, 0, 0.2);
  width: 100%;

  div.left {
    align-items: start;
  }

  div.right {
    align-items: end;
  }

  .dashboard {
    font-size: medium;
    background-color: rgba(14, 161, 101, 1);
    border-radius: 10px;
    padding: 8px 15px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  .dashboard:hover {
    background-color: rgba(14, 161, 101, 0.5);
  }

  h1.title {
    color: white;
    transition: color 0.3s ease;
    font-family: "Trebuchet MS", "Lucida Sans Unicode", "Lucida Grande",
      "Lucida Sans", Arial, sans-serif;
  }
  h1.title:hover {
    color: rgba(14, 161, 101, 1);
  }
}
</style>
