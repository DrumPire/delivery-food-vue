<template>
  <header class="header">
      <div class="header-box">
        <router-link to="/"><img src="../assets/img/logo.png" alt="Logotype" class="logo"></router-link>
        <div class="button-group">
          <button class="button button-main">
            <img src="../assets/img/icon-signin.svg" alt="Human icon">
            <span class="button-text">Войти</span>
          </button>
          <button class="button button-basket" @click="openModal()">
            <img src="../assets/img/icon-basket.svg" alt="Busket icon">
            <span class="button-text">Корзина</span>
          </button>
        </div>
      </div>
    </header>
</template>

<script setup>
  const emit = defineEmits(['toggleModal'])
  const openModal = () => emit('toggleModal')
</script>

<style scoped>
  .header {
    padding-top: 44px;
    padding-bottom: 22px;
  }
  .header-box {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  .banner {
  margin-bottom: 56px;
  }
  .banner-item {
    background-image: url("../assets/img/banners/banner.png");
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center right;
    padding: 68px 70px;
    border-radius: 10px;
    background-color: #fff1b8;
  }
  .banner-item_title {
    color: #302c34;
    font-size: 39px;
    font-weight: 700;
    max-width: 50%;
    margin-bottom: 15px;
  }
  .banner-item_subtitle {
    color: #302c34;
    font-size: 24px;
    max-width: 50%;
  }
</style>