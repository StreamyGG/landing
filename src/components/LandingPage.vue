<script lang="ts">
</script>

<template>
  <div class="landing">
    <img src="../assets/img/icon.webp" class="icon" />
    <h1>Best Multi-Streaming Bot</h1>
    <p>Seamlessly multistream to different platforms, while only having to add your widgets, chatbot rules, moderation and more only once!</p>
  </div>
</template>

<style lang="scss">
.landing {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 115px;
  text-align: center;

  .icon {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    animation: pulseUpDown 2s infinite;
  }

  @keyframes pulseUpDown {
    0%, 100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-10px); 
    }
  }

  h1 {
    margin: 15px 0 0;
    color: white;
    font-weight: 700;
  }

  p {
    margin: 5px 0 0;
    width: 30rem;
  }
} 
</style>