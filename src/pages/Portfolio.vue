<template>
  <q-page class="bg-grey-2">
    <section class="relative-position">
      <div class="effect-wrap">
        <div class="effect effect-1 absolute"></div>
        <div class="effect effect-2 absolute">
          <div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div>
        </div>
        <!-- <div class="effect effect-4 absolute"></div> -->
        <div class="effect effect-5 absolute">
          <div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div>
        </div>
      </div>
      <div class="row justify-center items-center q-pt-xl">
        <div class="col-9">
          <div class="row q-py-lg q-col-gutter-md justify-center">
            <div class="col-9 text-center">
              <div>You can see my lasts projects here, You can also type the technology or framework name below to find projects based on them. For confirmation of my role in projects, You can see my name at the bottom of them OR in codes. (for more information contact me)</div>
            </div>
            <div class="col-4">
              <q-input
                dense
                outlined
                rounded
                v-model="searchPortfolio" />
            </div>
            <div class="col-12" v-for="p in 12" :key="p">
              <q-card class="my-card bg-transparent" flat>
                <q-card-section horizontal>
                  <q-card-section class="col-5 flex flex-center">
                    <q-img
                      class="rounded-borders"
                      src="https://cdn.quasar.dev/img/parallax2.jpg"
                    />
                  </q-card-section>
                  <q-card-section>
                    <div class="text-overline">Overline</div>
                    <div class="text-h5 q-mt-sm q-mb-xs">Title</div>
                    <q-separator inset/>
                    <div class="text-caption text-grey">
                      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    </div>
                    <q-btn flat round icon="event" />
                    <q-btn flat>
                      7:30PM
                    </q-btn>
                    <q-btn flat color="primary">
                      Reserve
                    </q-btn>
                  </q-card-section>
                </q-card-section>
              </q-card>
            </div>
          </div>
        </div>
      </div>
    </section>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'PageIndex',
  data(){
    return{
      tabs: 'education'
    }
  }
})
</script>

<style lang="scss">
.img-box{
  max-width: 450px;
  border-radius: 50%;
  img{
    border-radius: 50%;
    box-shadow: inset 3px 3px 3px #d0d0d0, inset -3px -3px 3px #f8f8f8;
    border: 5px solid transparent;
  }
}
.home-text a,.about-info a,.social-links a,.box-service-item-icon{
  border-radius: 30px;
  transition: all 0.3s ease;
  &:after{
    border-radius: 30px;
  }
}
.effect-wrap .effect{
  z-index: 1
}
.effect-1{
  width: 30px;
  height: 30px;
  border: 4px solid #8a49ff;
  right: 15%;
  bottom: 10%;
  animation: spin 10s linear infinite
}
.effect-2{
  left: 6%;
  bottom: 20%;
  width: 40px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  animation: topBounce 3s ease-in-out infinite
}
.effect-2 div{
  height: 3px;
  width: 3px;
  background: #ff9c07;
  margin: 0 3px 8px;
}
.effect-4{
  border-top: 30px solid transparent;
  border-left: 30px solid #06d79c;
  left: 35%;
  top: 10%;
  animation: spin 15s linear infinite;
}
.effect-4:before{
  content: '';
  border-top: 30px solid transparent;
  border-left: 30px solid #06d79c;
  position: absolute;
  left: -35px;
  top: -25px;
  opacity: 0.5;
}
.effect-5{
  height: 50px;
  width: 50px;
  right: 10%;
  top: 25%;
  display: flex;
  justify-content: space-between;
  border-radius: 50px;
  overflow: hidden;
  animation: spin 10s linear infinite;
}
.effect-5 div{
  width: 4px;
  background: #4dd0e1;
}
@keyframes spin{
  0%{
    transform: rotate(0deg);
  }
  100%{
    transform: rotate(360deg);
  }
}
@keyframes topBounce{
  0%,100%{
    transform: translateY(0);
  }
  50%{
    transform: translateY(25px);
  }
}
.about-img{
  .img-box{
      border-radius: 0px; 
    img{
      border-radius: 0px
    }
  }
}
.btns-info{
  margin: 40px 0px;
  a:last-child{
    margin: 0px 15px;
  }
}
.social-links a{
  color: #9e9e9e;
}
.social-links a:hover,.service-item:hover .icon-service{
  color: #fb839e
}

.icon-service{
  &:after{
    content: '';
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    border-radius: 50%;
    transition: all 0.3s ease;
  }
}


.service-item:hover .box-service-item-icon{
  box-shadow: inset 0px 0px 0px #d0d0d0, inset 0px 0px 0px #f8f8f8;
  &:after{
    box-shadow: 3px 3px 3px #d0d0d0, -3px -3px 3px #f8f8f8;
  }
}

hr.q-separator.q-separator--horizontal{
  display: none;
}
.tab-line{
  .q-tab{
    border-radius: 30px;
    margin: 10px 0px;
    .q-focus-helper{
      background: transparent !important;
    }
  }
  .q-tab:hover{
    color: black;
  }
  .q-tab--active{
    border-radius: 30px;
    transition: all 0.3s ease;
    box-shadow: 3px 3px 3px #d0d0d0, -3px -3px 3px #f8f8f8;
    &:after{
      border-radius: 30px;
    }
  }
}
.skill-item span{
  top: -4px;
}
.r30{
  border-radius: 30px
}

.r10{
  border-radius: 10px
}
</style>
