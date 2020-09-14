<template>
  <div class="recomm__header">
    <div class="header__wrap">
      <img class="header__logo" width="37" height="37" src="~@/assets/Heart.svg" alt="logo" />
      <div class="text__wrap">
        <h2 class="header__title">Посоветуйте курс друзьям!</h2>
        <p class="header__tagline">Друзьям – знания, вам – рубли</p>
      </div>
      <button class="header__arrow" @click="visible=!visible"></button>
    </div>
    <div class v-show="visible">
      <div class="recomm__main">
        <p class="main__text">Рекомендуйте этот курс и получайте до 560 рублей с каждой покупки.</p>
      </div>
      <div class="recomm__social">
        <ul class="social__items">
          <li class="social__item--vk">
            <a href="#"></a>
          </li>
          <li class="social__item--fb">
            <a href="#"></a>
          </li>
          <li class="social__item--tw">
            <a href="#"></a>
          </li>
          <li class="social__item--ok">
            <a href="#"></a>
          </li>
          <li class="social__item--copy">
            <a href="#">
              Скопировать
              <br />ссылку
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Recommend",
  data() {
    return {
      visible: false
    };
  }
};
</script>

<style lang="scss">
.recomm__header {
  width: 360px;
  background: #f7f7f7;
}
.text__wrap {
  margin-top: 16px;
  margin-left: 10px;
}
.header__wrap {
  width: 325px;
  display: flex;
  margin: 0 auto;
}
.header__logo {
  margin-top: 18px;
}
.header__title {
  margin: 0;
  font-family: Open Sans, sans-serif;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  line-height: 20px;
  color: #000000;
}
.header__tagline {
  margin-top: 3px;
  text-align: left;
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 18px;
  color: #8d8d8d;
}
.header__arrow {
  position: relative;
  cursor: pointer;
  background: transparent;
  outline: none;
  border: none;
  margin-left: 48px;
  &::before {
    content: "";
    width: 15px;
    height: 15px;
    position: absolute;
    top: 28px;
    left: 0px;
    background-image: url("~@/assets/Group.svg");
    background-position: 0 0;
    background-repeat: no-repeat;
  }
}
.recomm__main {
  width: 295px;
  margin: 0 auto;
}
.main__text {
  font-size: 15px;
  line-height: 20px;
  text-align: left;
}
.recomm__social {
  width: 295px;
  padding-bottom: 34px;
  margin: 0 auto;
}
.social__items {
  display: flex;
  list-style: none;
  padding-left: 0px;
}
.social__item {
  width: 40px;
  height: 40px;
  position: relative;
  cursor: pointer;

  &--vk {
    width: 40px;
    height: 40px;
    cursor: pointer;
    background-image: url("~@/assets/Vk.svg");
    background-repeat: no-repeat;
    margin-right: 8px;
  }
  &--fb {
    width: 40px;
    height: 40px;
    cursor: pointer;
    background-image: url("~@/assets/F.svg");
    background-repeat: no-repeat;
    margin-right: 8px;
  }
  &--tw {
    width: 40px;
    height: 40px;
    cursor: pointer;
    background-image: url("~@/assets/Twit.svg");
    background-repeat: no-repeat;
    margin-right: 8px;
  }
  &--ok {
    width: 40px;
    height: 40px;
    cursor: pointer;
    background-image: url("~@/assets/Ok1.svg");
    background-repeat: no-repeat;
    margin-right: 8px;
  }
  &--copy {
    width: 89px;
    height: 40px;
    background-image: url("~@/assets/link1.svg");
    background-repeat: no-repeat;
    & > a {
      text-decoration: none;
      padding-left: 17px;
      color: #0069a4;
    }
  }
}
</style>
