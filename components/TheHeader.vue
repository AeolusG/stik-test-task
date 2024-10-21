<template>
  <div class="header">
    <div class="header-logo">
      <img src="../assets/stikLogo.png" alt="logo" />
    </div>
    <div class="bread-crumbs">
      <img src="../assets/Search.png" alt="Search" />
      <img src="../assets/Stroke.png" alt="Stroke" />
      <img src="../assets/User.png" alt="User" />
      <img src="../assets/Basket.png" alt="Basket" />
    </div>
    <div class="mobile-bread-crumbs">
      <img src="../assets/User.png" alt="User" />
      <img src="../assets/Search.png" alt="Search" />
      <div class="mobile-header-logo">
        <img src="../assets/stikLogo.png" alt="logo" />
      </div>
      <img src="../assets/Stroke.png" alt="Stroke" />
      <img src="../assets/Basket.png" alt="Basket" />
    </div>
  </div>
</template>

<style scoped>
body {
  margin: 0;
}
.header {
  display: flex;
  align-items: center;
  height: 86px;
}
.header-logo {
  margin-left: auto;
}
.bread-crumbs {
  margin-left: auto;
}
.mobile-bread-crumbs {
  display: none;
}
.mobile-header-logo {
  display: none;
}
@media screen and (max-width: 650px) {
  .header {
    display: flex;
    align-items: center;
    height: 86px;
  }
  .bread-crumbs {
    display: none;
  }
  .header-logo {
    display: none;
  }
  .mobile-bread-crumbs {
    display: flex;
    width: 100vw;
    justify-content: center;
  }
  .mobile-header-logo {
    display: flex;
    flex-grow: 1;
    justify-self: flex-start;
  }
  .mobile-header-logo img {
    margin: auto;
  }
}
</style>
