<script setup>
import { RouterLink } from 'vue-router';
</script>

<template>
  <div class="about">
    <h1>About Me</h1>
    <p class="desc">Copyright By
      <a href="https://instagram.com/_moneqa?igshid=MzNlNGNkZWQ4Mg==">
        <span class="owner">@Ry Sarakmony</span>
      </a>
    </p>
    <div class="bg">
      <img class="bg-pro" src="../assets/pfp.jpg" alt="logo" />
      <div class="bg_desc">
        <p class="bg-desc">- Hello World</p>
        <!-- <p class="bg-desc">- Age : 22 Years Old</p>
        <p class="bg-desc">- Study : IT at Build Bright Uni.</p>
        <p class="bg-desc">- Skill : Front End Engineer</p> -->
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@media (min-width: 1024px) {
  .about {
    /* min-height: 100vh; */
    display: flex;
    padding: 25px 16px;
    margin: 60px;
    flex-direction: column;

    .desc {
      margin-top: 20px;

      .owner {
        color: #333;
        text-decoration: underline;
      }

      .owner:hover {
        color: #41b080;
        cursor: pointer;
      }
    }

    .bg-pro {
      width: 300px;
      height: 300px;
      object-fit: cover;
      margin-top: 20px;
      border-radius: 3px;
    }
  }
}

.bg {
  display: flex;
  gap: 20px;
}

.about {
  margin: 20px;

  .bg-pro {
    width: 300px;
    height: 300px;
    border: #41b080 solid 3px;
    object-fit: cover;
    margin-top: 20px;
    border-radius: 3px;
  }

  .bg_desc {
    display: flex;
    flex-direction: column;
    margin-top: 30px;

    .bg-desc {
      font-size: 16px;
      padding-bottom: 9px;
    }
  }
}
</style>
