<template>
  <div>
    <div class="weui-tab">
      <div class="weui-tab__panel panel">
        <div>Page 1</div>
      </div>
      <div class="weui-tabbar tabbar">
        <a
          href="#"
          v-for="(item,index) in nav"
          :key="index"
          class="weui-tabbar__item weui-bar__item_on"
        >
          <img src="../assets/img/home.png" alt class="weui-tabbar__icon" />
          <p class="weui-tabbar__label">首页</p>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nav: [
        {
          href: "#",
          path: "../assets/img/home.png",
          name: "首页"
        },
        {
          href: "#",
          path: "../assets/img/circle.png",
          name: "分类"
        },
        {
          href: "#",
          path: "../assets/img/cart.png",
          name: "购物车"
        },
        {
          href: "#",
          path: "../assets/img/my.png",
          name: "我的"
        }
      ]
    };
  }
};
</script>

<style>
.panel {
  padding-bottom: 72px;
}
.tabbar {
  width: 375px;
  bottom: 0px;
  position: fixed;
}
</style>