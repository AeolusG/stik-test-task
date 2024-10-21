<template>
  <div class="card-content">
    <swiper
      :navigation="true"
      :modules="modules"
      :pagination="true"
      class="mySwiper"
    >
      <swiper-slide><img src="../assets/coat.png" alt="Coat" /></swiper-slide>
      <swiper-slide><img src="../assets/coat.png" alt="Coat" /></swiper-slide
      ><swiper-slide><img src="../assets/coat.png" alt="Coat" /></swiper-slide>
      <swiper-slide>
        <img class="" src="../assets/coat.png" alt=""
      /></swiper-slide>
    </swiper>
    <div class="product-promo">
      <img src="../assets/Image.png" alt="Coat" />
      <img src="../assets/Image (1).png" alt="Coat" />
      <img src="../assets/Image (2).png" alt="Coat" />
    </div>
    <div class="main-photo">
      <img class="" src="../assets/coat.png" alt="" />
    </div>
    <div class="purchase-info">
      <h4 class="purchase-text">ЖАКЕТ УДЛИНЁННЫЙ, БЕЛЫЙ</h4>
      <h5 class="purchase-text">8900 RUB</h5>
      <div class="sizes-title">Размеры</div>
      <div class="size-peaker">
        <div class="size-peaker-cotainer">
          <button class="size-peaker-btn">XS</button>
          <p class="size-peaker-note">Мало</p>
        </div>
        <div class="size-peaker-cotainer">
          <button class="size-peaker-btn">S</button>
        </div>
        <div class="size-peaker-cotainer">
          <button class="size-peaker-btn">M</button>
          <p class="size-peaker-note">Подписка</p>
        </div>
      </div>
      <div class="color-title">Цвет: белый</div>
      <div class="product-color-container">
        <button class="product-color product-color__white"></button>
        <button class="product-color product-color__black"></button>
        <button class="product-color product-color__beige"></button>
      </div>
      <div class="purchase-btns">
        <button class="add-basket-btn">Добавить в корзину</button>
        <button class="subscribe-btn">
          <img src="../assets/Active.png" />
        </button>
      </div>
      <div class="additional-btns">
        <div class="additonal-btns__container">
          <button class="usage-btn">Описание</button>
          <div>
            <img src="../assets/Plus.png" />
          </div>
        </div>
        <div class="additonal-btns__container">
          <button class="usage-btn">Состав и уход</button>
          <div>
            <img src="../assets/Plus.png" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { Navigation, Pagination } from "swiper";

import { SwiperCore, Swiper, SwiperSlide } from "swiper-vue2";

import "swiper/swiper-bundle.css";

SwiperCore.use([Navigation, Pagination]);

export default {
  name: "TheCard",
  data() {
    return {
      modules: [Navigation, Pagination],
    };
  },
  components: {
    Swiper,
    SwiperSlide,
  },
};
</script>

<style scoped>
.mySwiper {
  display: none;
}
.card-content {
  display: flex;
  margin-bottom: 40px;
}
.product-promo {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 10px;
  color: #828282;
  font-weight: 400;
  margin-right: 30px;
  cursor: pointer;
  display: flex;
  flex-direction: column;
}
.product-promo img {
  margin-bottom: 4px;
}
.main-photo {
  margin-right: 30px;
}
.color-title {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 10px;
  color: #4f4f4f;
  font-weight: 400;
  margin-bottom: 6px;
}
.sizes-title {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 10px;
  color: #828282;
  font-weight: 400;
  margin-bottom: 8px;
}
.size-peaker {
  display: flex;
}
.size-peaker-btn {
  border: 1px solid black;
  background: none;
  margin-right: 14px;
  padding: 9px 27px;
  margin-bottom: 3px;
}
.size-peaker-cotainer {
  margin-bottom: 36px;
}
.size-peaker-note {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 10px;
  color: #828282;
  font-weight: 400;
}
.product-color {
  height: 28px;
  width: 28px;
  border: none;
  margin: 0;
  margin-right: 16px;
}
.product-color-container {
  margin-bottom: 36px;
}
.product-color:focus::after {
  display: block;
  margin-top: 30px;
  margin-left: -9px;
  height: 1px;
  background-color: #4f4f4f;
  content: "";
  width: 34px;
}
.product-color__white {
  background-color: #ffffff;
  border: 1px #bdbdbd solid;
}
.product-color__black {
  background-color: #000000;
}
.product-color__beige {
  background-color: #f9f1dc;
}
.product-color--active {
  margin: 0;
  border-bottom: 1px solid black;
}
.purchase-text {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 12px;
  text-transform: uppercase;
  color: #333333;
  font-weight: 400;

  margin: 0;
  margin-bottom: 8px;
}

.purchase-btns {
  display: flex;
  min-width: 360px;
  align-items: center;
  margin-bottom: 40px;
}
.add-basket-btn {
  padding: 15px 0;
  color: white;
  background-color: black;
  border: none;
  font-size: 11px;
  text-transform: uppercase;
  flex-grow: 1;
  margin-right: 10px;
}
.subscribe-btn {
  border: none;
  background: none;
  height: 44px;
}
.usage-btn {
  border: none;
  background: none;
  padding: 15px 0;
  text-align: left;
}
.additional-btns {
  display: flex;
  flex-direction: column;
  margin-bottom: 40px;
}

.additonal-btns__container {
  display: flex;
  justify-content: space-between;
  border-top: solid #e0e0e0 1px;
  border-bottom: solid #e0e0e0 1px;
  align-items: center;
  margin-bottom: -1.2px;
  max-width: 360px;
}

@media screen and (max-width: 650px) {
  .card-content {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  .main-photo {
    display: none;
  }
  .product-promo {
    display: none;
  }
  .purchase-info {
    width: 100%;
    margin-left: 5px;
    margin-right: 5px;
  }
  .additonal-btns__container {
    max-width: none;
  }

  .mySwiper {
    display: block;
    margin-bottom: 30px;
  }
}
</style>
