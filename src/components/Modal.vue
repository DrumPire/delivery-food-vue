<template>
  <div class="cart-modal__overlay" :class="{open: isOpen}" @click.self="closeModal()">
      <div class="cart-modal">
        <div class="cart-modal__header">
          <h2 class="cart-modal__header--title">Корзина</h2>
          <span class="cart-modal__header--close" @click="closeModal()"><img src="../assets/img/close.svg" alt="Icon close"></span>
        </div>
        <div class="cart-modal__body">
          <div class="cart-item">
            <p class="cart-item__title">
              Ролл угорь стандарт
            </p>
            <div class="cart-item__controls">
              <p class="cart-item__controls--price">250 ₽</p>
              <button class="button button-basket modal-btn">-</button>
              <span class="cart-item__controls--count">1</span>
              <button class="button button-basket modal-btn">+</button>
            </div>
          </div>
          <div class="cart-item">
            <p class="cart-item__title">
              Ролл угорь стандарт
            </p>
            <div class="cart-item__controls">
              <p class="cart-item__controls--price">250 ₽</p>
              <button class="button button-basket modal-btn">-</button>
              <span class="cart-item__controls--count">1</span>
              <button class="button button-basket modal-btn">+</button>
            </div>
          </div>
          <div class="cart-item">
            <p class="cart-item__title">
              Ролл угорь стандарт
            </p>
            <div class="cart-item__controls">
              <p class="cart-item__controls--price">250 ₽</p>
              <button class="button button-basket modal-btn">-</button>
              <span class="cart-item__controls--count">1</span>
              <button class="button button-basket modal-btn">+</button>
            </div>
          </div>
          <div class="cart-item">
            <p class="cart-item__title">
              Ролл угорь стандарт
            </p>
            <div class="cart-item__controls">
              <p class="cart-item__controls--price">250 ₽</p>
              <button class="button button-basket modal-btn">-</button>
              <span class="cart-item__controls--count">1</span>
              <button class="button button-basket modal-btn">+</button>
            </div>
          </div>
        </div>
        <div class="cart-modal__footer">
          <div class="cart-modal__footer--price">
            1250 ₽
          </div>
          <div class="cart-modal__footer--controls">
            <button class="button button-main">
              <span class="button-text">Оформить заказ</span>
            </button>
            <button class="button button-basket">
              <span class="button-text">Отмена</span>
            </button>
          </div>
        </div>
      </div>
  </div>
</template>

<script setup>
  const {isOpen} = defineProps({isOpen: Boolean})
  const emit = defineEmits(['toggleModal'])
  const closeModal = () => emit('toggleModal')
</script>

<style scoped>
  .cart-modal {
    max-width: 780px;
    width: 100%;
    padding: 40px 45px;
    border-radius: 5px;
    background: #fff;
  }
  .cart-modal__overlay {
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.4);
    display: none;
    align-items: center;
    justify-content: center;
  }
  .cart-modal__overlay.open {
    display: flex;
  }
  .cart-modal__header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 45px;
  }
  .cart-modal__header--title {
    font-size: 36px;
    font-weight: 700;
    color: #000;
  }
  .cart-modal__header--close {
    cursor: pointer;
  }
  .cart-modal__footer {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 50px;
  }
  .cart-modal__footer--price {
    border-radius: 5px;
    padding: 0px 20px;
    color: #fafafa;
    font-size: 20px;
    background: #262626;
  }
  .cart-modal__footer--controls {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 10px;
  }
</style>