<template>
  <div>
    <slot></slot>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Emit } from 'vue-property-decorator';

@Component
export default class Scroll extends Vue {
  private state: number = 0; // 0 = 滚动中 1 = 滚动加载中 -1 = 滚动结束

  protected mounted() {
    console.log('mounted');
  }

  @Emit('load')
  private loading() {
    console.log('load');
  }
}
</script>
