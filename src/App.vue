<template>
  <div id="app" class="container">
    <div class="row mt-4">
      <div class="col-12 col-md-6 d-flex flex-column">
        <h1 class="text-primary mb-4">B站评论转图片</h1>
        <div class="flex-grow-1">
          <img
            class="d-none d-md-block"
            src="./assets/images/j9rSZOk.png"
            alt=""
          />
        </div>
      </div>
      <div class="col-12 col-md-6 d-flex flex-column">
        <img
          class="d-block img-rounded-corners"
          src="./assets/images/BilibiliBVId.gif"
          alt="获取BV示例"
        />
        <h5>功能：</h5>
        <ul>
          <li>不限制评论获取上限</li>
          <li>可调整评论区渲染样式</li>
          <li>支持打包为 ZIP 下载</li>
          <li>评论内容即文件名称</li>
        </ul>
      </div>
    </div>
    <hr />
    <div>
      <get-comments />
      <main-area />
    </div>
  </div>
</template>

<script>
import GetComments from "@/components/GetComments.vue";
import MainArea from "@/components/MainArea.vue";

export default {
  name: "App",
  components: {
    GetComments,
    MainArea,
  },
};
</script>

<style>
.img-rounded-corners {
  border: 1px solid #00a1d6;
  border-radius: 10px;
  margin: 0.625rem 0;
  opacity: 0.5;
  width: 100%;
}
</style>
