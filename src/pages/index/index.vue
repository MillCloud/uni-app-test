<template>
  <view class="container justify-center align-center h-full">
    <image class="logo" src="/static/logo.png" />
    <text class="text-20 my-20">
      {{ title }}
    </text>
    <button class="btn is-primary" @click="handleToPermission">测试权限</button>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: 'Hello, uni-app!',
    };
  },
  methods: {
    handleToPermission() {
      uni.navigateTo({
        url: '/pages/permission/index',
      });
    },
  },
};
</script>

<style lang="scss" scoped>
.logo {
  width: 492rpx;
  height: 120rpx;
}
</style>
