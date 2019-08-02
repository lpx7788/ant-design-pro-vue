<template>
  <div class="logo">
    <router-link :to="{name:'dashboard'}">
      <img src="../../assets/logo.png" style="width:28px;height:28px" alt="">
      <h1 v-if="showTitle">{{ title }}</h1>
    </router-link>
  </div>
</template>

<script>

export default {
  name: 'Logo',
  props: {
    title: {
      type: String,
      default: 'AIO商城后台',
      required: false
    },
    showTitle: {
      type: Boolean,
      default: true,
      required: false
    }
  }
}
</script>
