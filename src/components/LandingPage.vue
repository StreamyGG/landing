<script setup lang="ts"></script>

<template>
  <div class="landing">
    <img src="/icon.webp" class="icon" />
    <h1>Best Multi-Streaming Tool</h1>
    <p>
      Seamlessly multistream to different platforms, while only having to add
      your widgets, chatbot rules, moderation and more once!
    </p>
    <div class="socials">
      <a
        href="https://discord.gg/zUHH4VTTUh"
        target="_blank"
        rel="noopener noreferrer"
      >
        <h1 class="discord">
          <font-awesome-icon :icon="['fab', 'discord']" />&nbsp;&nbsp;Discord
        </h1>
      </a>
      <a
        href="https://x.com/streamygg"
        target="_blank"
        rel="noopener noreferrer"
      >
        <h1 class="twitter">
          <font-awesome-icon :icon="['fab', 'twitter']" />&nbsp;&nbsp;Twitter
        </h1>
      </a>
      <a
        href="https://github.com/StreamyGG"
        target="_blank"
        rel="noopener noreferrer"
      >
        <h1 class="github">
          <font-awesome-icon :icon="['fab', 'github']" />&nbsp;&nbsp;GitHub
        </h1>
      </a>
      <a
        href="https://ko-fi.com/bryden"
        target="_blank"
        rel="noopener noreferrer"
      >
        <h1 class="donate">
          <font-awesome-icon
            :icon="['fas', 'circle-dollar-to-slot']"
          />&nbsp;&nbsp;Donate
        </h1>
      </a>
    </div>
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
    0%,
    100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-10px);
    }
  }

  h1 {
    margin: 15px 11px 11px;
    color: white;
    font-weight: 700;
  }

  p {
    margin: 0 10px 10px;
    max-width: 30rem;
  }

  div.socials {
    margin: 0 10px 10px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;

    .discord {
      font-size: medium;
      background-color: rgba(88, 101, 242, 1);
      border-radius: 10px;
      padding: 8px 15px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .discord:hover {
      background-color: rgba(88, 101, 242, 0.5);
    }

    .donate {
      font-size: medium;
      background-color: rgba(14, 161, 101, 1);
      border-radius: 10px;
      padding: 8px 15px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .donate:hover {
      background-color: rgba(14, 161, 101, 0.5);
    }

    .twitter {
      font-size: medium;
      background-color: rgba(29, 161, 242, 1);
      border-radius: 10px;
      padding: 8px 15px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .twitter:hover {
      background-color: rgba(29, 161, 242, 0.5);
    }

    .github {
      font-size: medium;
      background-color: rgba(36, 41, 46, 1);
      border-radius: 10px;
      padding: 8px 15px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      color: white;
    }

    .github:hover {
      background-color: rgba(36, 41, 46, 0.5);
    }
  }

  @media (max-width: 5px) {
    div.socials {
      flex-direction: column;
      align-items: center;
    }
  }
}
</style>
