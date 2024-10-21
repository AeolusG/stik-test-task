<template>
  <article class="wrapper">
    <h5 class="more-info-title">Похожие товары</h5>
    <div class="similar-goods-container">
      <div class="similar-good">
        <img src="../assets/good1.png" />
        <p class="similar-good-title">ПЛАТЬЕ С V-ОБРАЗНЫМ ВЫРЕЗОМ, БЕЛЫЙ</p>
        <div class="similar-good-sale-container">
          <p class="similar-good-price">14 900 RUB</p>
          <p class="similar-good-sale">18 000 RUB</p>
        </div>
      </div>
      <div class="similar-good">
        <img src="../assets/good2.png" />
        <p class="similar-good-title">ПЛАТЬЕ С V-ОБРАЗНЫМ ВЫРЕЗОМ, БЕЛЫЙ</p>
        <div class="similar-good-sale-container">
          <p class="similar-good-price">14 900 RUB</p>
        </div>
      </div>
      <div class="similar-good">
        <img src="../assets/good3.png" />
        <p class="similar-good-title">ПЛАТЬЕ С V-ОБРАЗНЫМ ВЫРЕЗОМ, БЕЛЫЙ</p>
        <div class="similar-good-sale-container">
          <p class="similar-good-price">14 900 RUB</p>
        </div>
      </div>
      <div class="similar-good">
        <img src="../assets/good4.png" />
        <p class="similar-good-title">ПЛАТЬЕ С V-ОБРАЗНЫМ ВЫРЕЗОМ, БЕЛЫЙ</p>
        <div class="similar-good-sale-container">
          <p class="similar-good-price">14 900 RUB</p>
        </div>
      </div>
    </div>
    <div class="mobile-similar-goods-container">
      <div class="similar-good">
        <img src="../assets/good1.png" />
        <p class="similar-good-title">ПЛАТЬЕ С V-ОБРАЗНЫМ ВЫРЕЗОМ, БЕЛЫЙ</p>
        <div class="similar-good-sale-container">
          <p class="similar-good-price">14 900 RUB</p>
          <p class="similar-good-sale">18 000 RUB</p>
        </div>
      </div>
      <div class="similar-good">
        <img src="../assets/good2.png" />
        <p class="similar-good-title">ПЛАТЬЕ С V-ОБРАЗНЫМ ВЫРЕЗОМ, БЕЛЫЙ</p>
        <div class="similar-good-sale-container">
          <p class="similar-good-price">14 900 RUB</p>
        </div>
      </div>
    </div>
    <div class="mobile-similar-goods-container">
      <div class="similar-good">
        <img src="../assets/good3.png" />
        <p class="similar-good-title">ПЛАТЬЕ С V-ОБРАЗНЫМ ВЫРЕЗОМ, БЕЛЫЙ</p>
        <div class="similar-good-sale-container">
          <p class="similar-good-price">14 900 RUB</p>
        </div>
      </div>
      <div class="similar-good">
        <img src="../assets/good4.png" />
        <p class="similar-good-title">ПЛАТЬЕ С V-ОБРАЗНЫМ ВЫРЕЗОМ, БЕЛЫЙ</p>
        <div class="similar-good-sale-container">
          <p class="similar-good-price">14 900 RUB</p>
        </div>
      </div>
    </div>
  </article>
</template>

<style scoped>
body {
  margin: 0;
}
.wrapper {
  margin-bottom: 40px;
}
.more-info-title {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 12px;
  text-transform: uppercase;
  color: #333333;
  font-weight: 400;

  margin: 0;
  margin-bottom: 30px;
}
.similar-goods-container {
  display: flex;
}
.similar-good {
  margin-right: 8px;
}
.similar-good img {
  margin-bottom: 15px;
}
.similar-good-title {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 10px;
  color: #333333;
  font-weight: 400;
  margin-bottom: 10px;
}
.similar-good-price {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 10px;
  color: #333333;
  font-weight: 400;
  margin-bottom: 10px;
  margin-right: 10px;
  margin-top: 0;
}
.similar-good-sale {
  display: inline;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 10px;
  color: #828282;
  margin-top: 0;
  text-decoration: line-through;
}
.similar-good-sale-container {
  display: flex;
}
.mobile-similar-goods-container {
  display: none;
}
@media screen and (max-width: 650px) {
  .similar-goods-container {
    display: flex;
    flex-wrap: wrap;
  }
  .mobile-similar-goods-container {
    display: flex;
    justify-content: center;
  }
  .similar-goods-container {
    display: none;
  }
  .similar-good img {
    width: 49vw;
  }
  .similar-good {
    margin-right: 0;
  }
}
</style>
