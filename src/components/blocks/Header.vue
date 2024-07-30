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
  padding: 5px 25px;
  border-bottom: 0.25px solid black;
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
  }
  h1.title:hover {
    color: rgba(14, 161, 101, 1);
  }
}
</style>
