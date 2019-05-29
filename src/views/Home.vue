<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
    <scroll></scroll>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import Scroll from '@/components/scroll/scroll.vue';
@Component({
  components: {
    HelloWorld,
    Scroll,
  },
})
export default class Home extends Vue {}
</script>
