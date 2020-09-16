<template>
  <div id="app">
    <Recommend :msg="msg" :urls="urls" />
  </div>
</template>

<script>
import Recommend from '@/components/Recommend';

export default {
  name: 'App',
  data() {
    return {
      urls: [
        {
          name: 'Vk',
          img: '/Vk.svg',
          src: 'https://vk.com/share.php?url=http://mysite.com',
        },
        {
          name: 'Ok',
          img: '/Ok1.svg',
          src: 'https://connect.ok.ru/offer?url=http://mysite.com',
        },
        {
          name: 'Twit',
          img: '/Twit.svg',
          src: 'https://vk.com/share.php?url=http://mysite.com',
        },
        {
          name: 'Fb',
          img: '/F.svg',
          src: 'https://vk.com/share.php?url=http://mysite.com',
        },
      ],
      msg: 'Hi',
    };
  },
  components: {
    Recommend,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
