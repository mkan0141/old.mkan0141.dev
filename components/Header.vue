<template>
  <header class="flex justify-between items-center md:mx-56 md:mt-6">
    <div class="text-4xl text-black">
      mkan0141.dev
    </div>
    <nav class="">
      <ul class="flex">
        <li class="text-2xl hover:text-blue" :class="{ 'text-blue': activityMenuType === MenuType.Top}" v-on:click="onClickMenu(MenuType.Top)">
          <nuxt-link to="/">Top</nuxt-link>
        </li>
        <li class="ml-8 text-2xl hover:text-puple" :class="{ 'text-puple': activityMenuType === MenuType.Profile}" v-on:click="onClickMenu(MenuType.Profile)">
          <nuxt-link to="/Profile">Profile</nuxt-link>
        </li>
        <li class="ml-8 text-2xl hover:text-green" :class="{ 'text-green': activityMenuType === MenuType.Works}" v-on:click="onClickMenu(MenuType.Works)">
          <nuxt-link to="/Works">Works</nuxt-link>
        </li>
        <li class="ml-8 text-2xl hover:text-skyblue" :class="{ 'text-skyblue': activityMenuType === MenuType.Blog }" v-on:click="onClickMenu(MenuType.Blog)">
          <nuxt-link to="/">Blog</nuxt-link>
        </li>
      </ul>
    </nav>
  </header>  
</template>

<script lang="ts">
import Vue from 'vue'

enum MenuType {
  Top,
  Profile,
  Works,
  Blog,
}

export default Vue.extend({
  data() {
    return {
      activityMenuType: MenuType.Top,
    }
  },
  methods: {
    onClickMenu (menuType: MenuType) {
      this.activityMenuType = menuType
    }
  },
  computed: {
    MenuType () {
      return MenuType
    }
  }
})
</script>

<style lang="scss">
header {
  font-family:  'M PLUS Rounded 1c', sans-serif;
}
</style>