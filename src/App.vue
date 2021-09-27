<template>
  <router-view />
</template>
<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App'
})
</script>

<style lang="scss">
a{
  text-decoration: none;
}
.outer-shadow{
 box-shadow: 3px 3px 3px #d0d0d0, -3px -3px 3px #f8f8f8;
}
.outer-shadow-0{
 box-shadow: 0px 0px 0px #d0d0d0, 0px 0px 0px #f8f8f8;
}  
.inner-shadow{
  box-shadow: inset 3px 3px 3px #d0d0d0, inset -3px -3px 3px #f8f8f8;
}
.inner-shadow-0{
  box-shadow: inset 0px 0px 0px #d0d0d0, inset 0px 0px 0px #f8f8f8;
}
.hover-in-shadow{
  position: relative;
  z-index: 1;
}
.hover-in-shadow:hover{
  box-shadow: 0px 0px 0px #d0d0d0, 0px 0px 0px #f8f8f8;
}
.hover-in-shadow:after{
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  transition: all 0.3 ease;
}
.hover-in-shadow:hover:after{
  box-shadow: inset 3px 3px 3px #d0d0d0, inset -3px -3px 3px #f8f8f8;
}
</style>