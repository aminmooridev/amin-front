<template>
  <q-page class="bg-grey-2 windows-height">
    <section class="home-section section q-py-lg relative-position">
      <div class="effect-wrap">
        <div class="effect effect-1 absolute"></div>
        <div class="effect effect-2 absolute">
          <div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div>
        </div>
        <div class="effect effect-4 absolute"></div>
        <div class="effect effect-5 absolute">
          <div></div><div></div><div></div><div></div><div></div><div></div><div></div><div></div>
        </div>
      </div>
      <div class="row justify-center">
        <div class="col-11 col-md-9">
          <div class="row items-center justify-between">
            <div class="col home-text q-gutter-y-md">
              <p>سلام</p>
              <div class="text-h3 text-weight-bold">امین موری</div>
              <div>طراح و توسعه دهنده وب</div>
              <div class="q-mt-lg">
                <a href="" class="outer-shadow hover-in-shadow text-primary q-py-sm q-px-lg cursor-pointer">
                  درباره ی من
                </a>
              </div>
            </div>
            <div class="col home-img q-px-md">
              <div class="img-box q-mx-auto inner-shadow q-pa-md">
                <q-img
                  src="image/man.png"
                  class="full-width"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="about-section section q-py-lg">
      <div class="row justify-center">
        <div class="col-11 col-md-9">
          <div class="row">
            <div class="section-title q-mx-auto text-center">
              <div class="text-primary">اطلاعات اصلی</div>
              <div class="text-h5 text-weight-bold">درباره من</div>
            </div>
          </div>
          <div class="row q-py-lg justify-between">
            <div class="col-5 about-img">
              <div class="q-gutter-y-md">
                <div class="img-box inner-shadow q-pa-md">
                  <q-img
                    src="image/man.png"
                    class="full-width"
                  />
                </div>
                <div class="social-links text-center q-gutter-x-sm">
                  <a class="outer-shadow hover-in-shadow q-pa-sm cursor-pointer text-center">
                    <q-icon name="fab fa-instagram" size="sm"/>
                  </a>
                  <a class="outer-shadow hover-in-shadow q-pa-sm cursor-pointer text-center">
                    <q-icon name="fab fa-twitter" size="sm"/>
                  </a>
                  <a class="outer-shadow hover-in-shadow q-pa-sm cursor-pointer text-center">
                    <q-icon name="fab fa-facebook" size="sm"/>
                  </a>
                  <a class="outer-shadow hover-in-shadow q-pa-sm cursor-pointer text-center">
                    <q-icon name="fab fa-telegram" size="sm"/>
                  </a>
                </div>
              </div>
            </div>
            <div class="col-6 about-info">
              <p><span class="text-weight-bold">سلام ! من امین موری ، طراح و توسعه دهنده سایت هستم.</span> لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد کتابهای زیادی در شصت و سه درصد گذشته حال و آینده</p>
              <p>لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد کتابهای زیادی در شصت و سه درصد گذشته حال و آینده</p>
              <div class="btns-info">
                <a class="outer-shadow hover-in-shadow text-primary q-py-sm q-px-lg cursor-pointer">دانلود رزومه</a>
                <a class="outer-shadow hover-in-shadow text-primary q-py-sm q-px-lg cursor-pointer">استخدام</a>
              </div>
            </div>
          </div>
          <div class="row">
            <div
              class="full-width"
            >
              <q-tabs
                v-model="tabs"
                dense
                class="text-grey tab-line"
                align="center"
                active-color="primary"
                indicator-color="transparent"
              >
                <q-tab name="skills" label="مهارت ها" />
                <q-tab name="education" label="تحصیلات" />
                <q-tab name="experience" label="تجربه ها" />
              </q-tabs>

              <q-separator />

              <q-tab-panels 
                v-model="tabs"
                animated
                transition-prev="fade"
                transition-next="fade"
                class="bg-transparent"
              >
                <q-tab-panel name="skills">
                  <div class="row q-col-gutter-y-lg q-col-gutter-x-md">
                    <div class="col-6">
                      <div class="skill-item q-gutter-y-xs relative-position">
                        <div class="text-grey-6">Html</div>
                        <span class="absolute" style="right: 46.5%">50%</span>
                        <div class="outer-shadow inner-shadow q-pa-sm r30">
                          <q-linear-progress size="6px" value="0.5" class="rounded-borders" color="grey-7"/>
                        </div>
                      </div>
                    </div>
                    <div class="col-6">
                      <div class="skill-item q-gutter-y-xs relative-position">
                        <div class="text-grey-6">Css</div>
                        <span class="absolute" style="right: 71%">50%</span>
                        <div class="outer-shadow inner-shadow q-pa-sm r30">
                          <q-linear-progress size="6px" value="0.75" class="rounded-borders" color="grey-7"/>
                        </div>
                      </div>
                    </div>
                    <div class="col-6">
                      <div class="skill-item q-gutter-y-xs relative-position">
                        <div class="text-grey-6">Css</div>
                        <span class="absolute" style="right: 71%">50%</span>
                        <div class="outer-shadow inner-shadow q-pa-sm r30">
                          <q-linear-progress size="6px" value="0.75" class="rounded-borders" color="grey-7"/>
                        </div>
                      </div>
                    </div>
                    <div class="col-6">
                      <div class="skill-item q-gutter-y-xs relative-position">
                        <div class="text-grey-6">Html</div>
                        <span class="absolute" style="right: 46.5%">50%</span>
                        <div class="outer-shadow inner-shadow q-pa-sm r30">
                          <q-linear-progress size="6px" value="0.5" class="rounded-borders" color="grey-7"/>
                        </div>
                      </div>
                    </div>
                  </div>
                </q-tab-panel>

                <q-tab-panel name="education" class="text-center">
                  <q-timeline layout="loose" color="primary">

                    <q-timeline-entry
                      title="Event Title"
                      side="left"
                      icon="school"
                    >
                      <div class="text-primary text-caption">February 22, 1986</div>
                      <div class="text-grey-5">February 22, 1986</div>
                      <div class="q-mt-sm">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                      </div>
                    </q-timeline-entry>

                    <q-timeline-entry
                      title="Event Title"
                      side="right"
                      icon="school"
                    >
                      <div class="text-primary text-caption">February 22, 1986</div>
                      <div class="text-grey-5">February 22, 1986</div>
                      <div class="q-mt-sm">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                      </div>
                    </q-timeline-entry>

                    <q-timeline-entry
                      title="Event Title"
                      side="left"
                      icon="school"
                    >
                      <div class="text-primary text-caption">February 22, 1986</div>
                      <div class="text-grey-5">February 22, 1986</div>
                      <div class="q-mt-sm">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                      </div>
                    </q-timeline-entry>

                    <q-timeline-entry
                      title="Event Title"
                      side="right"
                      icon="school"
                    >
                      <div class="text-primary text-caption">February 22, 1986</div>
                      <div class="text-grey-5">February 22, 1986</div>
                      <div class="q-mt-sm">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                      </div>
                    </q-timeline-entry>

                  </q-timeline>
                </q-tab-panel>

                <q-tab-panel name="experience">
                  <q-timeline layout="loose" color="primary">

                    <q-timeline-entry
                      title="Event Title"
                      side="left"
                      icon="school"
                    >
                      <div class="text-primary text-caption">February 22, 1986</div>
                      <div class="text-grey-5">February 22, 1986</div>
                      <div class="q-mt-sm">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                      </div>
                    </q-timeline-entry>

                    <q-timeline-entry
                      title="Event Title"
                      side="right"
                      icon="school"
                    >
                      <div class="text-primary text-caption">February 22, 1986</div>
                      <div class="text-grey-5">February 22, 1986</div>
                      <div class="q-mt-sm">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                      </div>
                    </q-timeline-entry>

                    <q-timeline-entry
                      title="Event Title"
                      side="left"
                      icon="school"
                    >
                      <div class="text-primary text-caption">February 22, 1986</div>
                      <div class="text-grey-5">February 22, 1986</div>
                      <div class="q-mt-sm">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                      </div>
                    </q-timeline-entry>

                    <q-timeline-entry
                      title="Event Title"
                      side="right"
                      icon="school"
                    >
                      <div class="text-primary text-caption">February 22, 1986</div>
                      <div class="text-grey-5">February 22, 1986</div>
                      <div class="q-mt-sm">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                      </div>
                    </q-timeline-entry>

                  </q-timeline>
                </q-tab-panel>
              </q-tab-panels>
            </div>
          </div>
        </div>
      </div>     
    </section>

    <section class="service-section section q-py-lg">
      <div class="row justify-center">
        <div class="col-11 col-md-9 q-gutter-y-lg">
          <div class="row">
            <div class="section-title q-mx-auto text-center">
              <div class="text-primary">خدمات من</div>
              <div class="text-h5 text-weight-bold">آنچه من انجام می دهم</div>
            </div>
          </div>
          <div class="row">
            <div class="col-12">
              <div class="row q-col-gutter-lg">
                <div class="col-4" v-for="ser in 6" :key="ser">
                  <div class="outer-shadow rounded-borders service-item cursor-pointer q-pt-lg q-pb-lg">
                    <q-card-section class="text-center">
                        <div class="text-h6 q-pt-md">
                          <span class="inner-shadow q-pa-md box-service-item-icon">
                            <q-icon name="phone_iphone" size="md" class="icon-service"/>
                          </span>
                        </div>
                    </q-card-section>
                    <q-card-section>
                      <div class="text-subtitle2 text-center text-bold">ریسپانسیو</div>
                    </q-card-section>
                    <q-card-section class="q-pt-none text-center">
                      لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است
                    </q-card-section>
                  </div>
                </div>
              </div>
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
