<template>
  <div id="app">
    <SoundSwitcher />
    <router-view/>
  </div>
</template>

<script>
import SoundSwitcher from '@/components/SoundSwitcher'

export default {
  name: 'App',
  components: {
    SoundSwitcher,
  },
}
</script>

<style>
html {
  font-size: 15.625vw;
}
#app {
  width: 100vw;
  height: 100vh;
  background-color: #000;
}
</style>
