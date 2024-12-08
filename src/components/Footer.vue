<template>
  <footer class="footer">
      <div class="header-box">
        <router-link to="/"><img src="../assets/img/logo.png" class="footer-logo" alt="Logotype"></router-link>
        <nav class="nav">
          <ul class="nav-list">
            <li class="nav-items">
              <a href="/goods.html">Ресторанам </a>
            </li>
            <li class="nav-items">
              <a href="/goods.html">Курьерам</a>
            </li>
            <li class="nav-items">
              <a href="/goods.html">Пресс-центр</a>
            </li>
            <li class="nav-items">
              <a href="/goods.html">Контакты</a>
            </li>  
          </ul>
        </nav>
        <div class="button-group">
          <a href="#" class="social">
            <img src="../assets/img/instagram.svg" alt="Instagram icon">
          </a>
          <a href="#" class="social">
            <img src="../assets/img/facebook.svg" alt="Facebook icon">
          </a>
          <a href="#" class="social">
            <img src="../assets/img/vk.svg" alt="VK icon">
          </a>
        </div>
      </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
  .footer {
    padding: 60px 0;
  }
  .footer-logo {
    margin-right: 35px;
  }
  .header-box {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  .social:not(:last-child) {
  margin-right: 21px;
  }

  .nav {
    margin-right: auto;
  }
  .nav-list {
    list-style: none;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  .nav-list a {
    text-decoration: none;
    font-size: 18px;
    color: #595959;
  }
  .nav-items:not(:last-child) {
    margin-right: 15px;
  }
</style>