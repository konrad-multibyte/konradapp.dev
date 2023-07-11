<template>
  <div class="flex">
    <div class="container">
      <div class="header">
        <h1 class="header-text text-3xl">Konrad Gladysz</h1>
      </div>
      <div class="profile">
        <img class="profile-img" src="/profile.png" />
        <p class="text-xl text-bold">Konrad Gladysz</p>
      </div>
      <div class="content-1">Content-1</div>
      <div class="content-2">Content-2</div>
      <div class="content-3">Content-3</div>
      <div class="footer">
        <a href="https://github.com/konrad-multibyte" target="_blank" rel="noopener noreferrer">
          <img class="github-footer-img" src="/GitHub_Logo.png" alt="GitHub logo">
        </a>
        <a href="https://ie.linkedin.com/in/konrad-gladysz" target="_blank" rel="noopener noreferrer">
          <img class="linkedin-footer-img" src="/LI-Logo.png" alt="LinkedIn logo">
        </a>
      </div>
      <style>
        .flex {
          display: flex;
          align-items: center;
          justify-content: center;

        }
        .container {
          display: grid;
          width: 100%;
          height: 100%;
          grid-template-columns: 200px 1fr 1fr;
          grid-template-rows: 80px 1fr 1fr 100px;
          grid-gap: 1rem;
        }

        .header {
          display: flex;
          align-items: center;
          justify-content: left;
          grid-row: 1 / 2;
          grid-column: 1 / 4;
        }

        .header-text {
          margin-left: 1em;
        }

        .profile {
          grid-row: 2 / 4;
          grid-column: 1 / 2;
          display: flex;
          flex-direction: column;
          align-items: center;
          justify-content: center;
        }

        .profile-img {
          border-radius: 25px;
        }

        .content-1 {
          grid-row: 2 / 3;
          grid-column: 2 / 4;
        }

        .content-2 {
          grid-row: 3 / 4;
          grid-column: 2 / 3;
        }

        .content-3 {
          grid-row: 3 / 4;
          grid-column: 3 / 4;
        }

        .footer {
          display: flex;
          grid-row: 4 / 5;
          grid-column: 1 / 4;
        }

        .github-footer-img {
          width: 500px;
          height: 102px;
        }

        .linkedin-footer-img {
          width: 500px;
          height: 110px;
        }

        * {
          border: 1px solid black;
        }
      </style>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage'
})
</script>
