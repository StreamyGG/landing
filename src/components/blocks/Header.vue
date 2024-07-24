<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
    <header>
        <div class="header">
         <div class="left">
            <RouterLink to="/">
              <h1><b style="font-weight: bold;">Streamy</b>Bot</h1>
            </RouterLink>
         </div>
         <div class="right">
            <a href="https://dash.streamybot.xyz" target="_blank" rel="noopener noreferrer">
                <h1 class="dashboard">Dashboard</h1>
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
       font-weight: bold;
       border: rgb(56, 58, 58);
       background-color: black;
       border-style: solid;
       border-radius: 10px;
       padding: 8px;
       cursor: pointer;
    }

    .dashboard:hover {
        background-color: transparent;
    }

    a {
        text-decoration: none;
        color: inherit;
      }

    a.router-link-exact-active {
        color: var(--color-text);
        text-decoration: none;
    }
      
     a.router-link-exact-active:hover {
        background-color: transparent;
    }
}
</style>