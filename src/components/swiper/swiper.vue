<template>
  <div>
    <slot></slot>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Emit } from 'vue-property-decorator';

@Component
export default class Swiper extends Vue {
  protected mounted() {
    console.log('mounted');
  }

  @Emit('load')
  private loading() {
    console.log('load');
  }
}
</script>
