<template>
  <div class="home">
    <HelloWorld msg="Welcome to My home"/>
    <div class="home2"></div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

@Options({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
  .home2 {
    width: 100%;
    height: 100px;
    background-color: red;
  }
</style>
