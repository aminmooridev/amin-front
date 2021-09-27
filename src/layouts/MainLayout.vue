<template>
  <q-layout view="hHh lpR fFf">

    <q-header class="bg-grey-2 relative-position">
      <div class="effect-wrap">
        <div class="effect effect-3 absolute"></div>
      </div>
      <div class="row justify-center q-py-md">
        <div class="col-11 col-md-9">
          <div class="row justify-between items-center">
            <!-- <div @click="navMenu = true" class="hamburger-btn justify-center items-center text-center cursor-pointer outer-shadow hover-in-shadow">
              <span></span>
            </div> -->
            <div class="logo">
              <a href="/" class="text-h6 text-primary text-center">
                ام
              </a>
            </div>
            <div class="btn-menus q-gutter-x-sm">
              <q-btn
                to="/"
                flat
                rounded
                label="صفحه ی اصلی"
                class="outer-shadow hover-in-shadow text-grey after-btn" />
              <q-btn
                to="/about"
                flat
                rounded
                label="درباره"
                class="outer-shadow hover-in-shadow text-grey after-btn" />
              <q-btn
                to="/portfolio"
                flat
                rounded
                label="مهارت ها"
                class="outer-shadow hover-in-shadow text-grey after-btn" />
              <q-btn
                flat
                rounded
                label="نمونه کار"
                class="outer-shadow hover-in-shadow text-grey after-btn" />
              <q-btn
                rounded
                label="تماس"
                color="primary"
                class="text-white after-btn"/>
            </div>
          </div>
        </div>
      </div>
      <!-- <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg">
          </q-avatar>
          Title
        </q-toolbar-title>
      </q-toolbar> -->
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-dialog
      v-model="navMenu"
      persistent
      transition-show="fade"
      transition-hide="fade"
      :maximized="true"
    >
      <q-card class="bg-grey-2 navMenu">
        <q-card-section class="text-left">
          <span class="outer-shadow hover-in-shadow items-center text-center" v-close-popup>
            <q-icon name="close" class="q-mx-auto" size="sm"/>
          </span>
        </q-card-section>

        <q-card-section class="flex flex-center text-center">
          <ul class="q-pa-md">
            <li class="q-mb-md"><a href="" class="inner-shadow active text-grey q-py-sm q-px-lg">Home</a></li>
            <li class="q-mb-md"><a href="" class="outer-shadow hover-in-shadow text-grey q-py-sm q-px-lg">About</a></li>
            <li class="q-mb-md"><a href="" class="outer-shadow hover-in-shadow text-grey q-py-sm q-px-lg">Services</a></li>
            <li class="q-mb-md"><a href="" class="outer-shadow hover-in-shadow text-grey q-py-sm q-px-lg">Portfolio</a></li>
            <li class="q-mb-md"><a href="" class="outer-shadow hover-in-shadow text-grey q-py-sm q-px-lg">Testimonial</a></li>
            <li><a href="" class="outer-shadow hover-in-shadow text-grey q-py-sm q-px-lg">Contact</a></li>
          </ul>
        </q-card-section>
      </q-card>
    </q-dialog>

  </q-layout>
</template>

<script>
export default {
  data() {
    return {
      navMenu: false
    }
  }
}
</script>

<style lang="scss">
.after-btn{
  &:after{
    border-radius: 28px;
  }
}
.logo a{
  height: 40px;
  width: 40px;
  border: 2px solid #fb839e !important;
  display: inline-block;
  line-height: 36px;
  border-radius: 50%;
  text-decoration: none;
}
.hamburger-btn,.navMenu span{
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  transition: all 0.3s ease;
  &:after{
    border-radius: 50%;
  }
  span{
    display: block;
    height: 2px;
    width: 16px;
    background: grey;
    position: relative;
    &:before,&:after {
        content: "";
        position: absolute;
        left: 0px;
        width: 100%;
        height: 100%;
        background: grey
    }
    &:before{
      top: -6px;
    }
    &:after{
      top: 6px;
    }
  }
}
.navMenu ul{
  list-style-type: none;
  a{
    display: inline-block;
    border-radius: 30px;
    transition: all 0.3s ease;
    &:after{
      border-radius: 30px;
    }
  }
}
.navMenu ul li a.active{
  color:#fb839e !important;
}
.effect-3{
  width: 180px;
  height: 180px;
  border: 25px solid #fb839e;
  border-radius: 50%;
  left: 50%;
  top: -120px;
  animation: leftBounce 3s ease-in-out infinite
}
@keyframes leftBounce{
  0%,100%{
    transform: translateX(0);
  }
  50%{
    transform: translateX(25px);
  }
}
</style>