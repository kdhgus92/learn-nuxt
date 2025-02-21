<template>
  <div>
    <header>
      <h1>{{ $route.name }} 페이지</h1>
      <NuxtLink to="/">홈페이지</NuxtLink>
      <NuxtLink to="/main">main페이지</NuxtLink>
      <NuxtLink to="/product">product페이지</NuxtLink>
    </header>
    <AppHeader />
    <Nuxt />
  </div>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';

export default {
  components: { AppHeader },
  created() {
    console.log(this.$route.name);
  },
};
</script>
