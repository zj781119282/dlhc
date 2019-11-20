<template>
  <i class="iconfont" :class="sound ? 'rotate' : ''" @click="sound = !sound">{{sound ? '&#xe990;' : '&#xe608;'}}</i>
</template>

<script>
export default {
  name: 'SoundSwitcher',
  data() {
    return {
      sound: true,
    }
  },
}
</script>

<style lang=scss scoped>
  .iconfont {
    position: fixed;
    right: 20px;
    top: 20px;
    font-size: 30px;
    color: rgb(1, 165, 175);
  }
  .rotate {
    animation: rotate 2s infinite linear;
  }
  @keyframes rotate {
    0% {
      transform: rotate(0);
    }
    50% {
      transform: rotate(180deg);
    }
    100% {
      transform: rotate(360deg);
    }
  }
</style>
