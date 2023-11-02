<script setup>
const titleLeftData = ['绿化', 'i很低啊', '哦是滴', '抗裂砂浆']
const titleRightData = ['绿化', 'i很低啊', '哦是滴', '抗裂砂浆']

const contentBarLeftData = ['考古所', '考试规定']
const contentBarMiddleData = ['考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定',]
const contentBarRightData = ['考古所', '考试规定', '考古所', '考试规定', '考古所', '考试规定',]

// 1111111111111111111111111111111111111111111111111111111111111111111
// 2222222222222222222222222222222222222222222222222222222222222222222
</script>

<template>
  <div class="page-title">
    <div class="title-left">
      <div class="title-left-item" v-for="item in titleLeftData" :key="item">{{ item }}</div>
    </div>
    <div class="title-middle">
      <input type="text">
    </div>
    <div class="title-right">
      <div class="title-right-item" v-for="item in titleRightData" :key="item">{{ item }}</div>
    </div>
  </div>
  <div class="page-main">
    <div class="page-main-content">
      <div class="main-content-bar">
        <div class="content-bar-left">
          <div class="bar-left-item" v-for="item in contentBarLeftData" :key="item">{{ item }}</div>
        </div>
        <div class="content-bar-middle">
          <div class="bar-middle-item" v-for="item in contentBarMiddleData" :key="item">{{ item }}</div>
        </div>
        <div class="content-bar-right">
          <div class="bar-right-item" v-for="item in contentBarRightData" :key="item">{{ item }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.page-title {
  display: flex;
  justify-content: space-between;
  height: 100px;
  width: 100%;
  background-color: aqua;

  .title-left {
    display: flex;

    .title-left-item {
      margin-left: 30px;
    }
  }

  .title-right {
    display: flex;

    .title-right-item {
      margin-right: 30px;
    }
  }
}

.page-main {
  width: 100%;
  display: flex;
  justify-content: center;

  .page-main-content {
    width: 90%;

    .main-content-bar {
      height: 100px;
      width: 100%;
      display: flex;

      .content-bar-left {
        width: 10%;
        background-color: aquamarine;
        display: flex;
        align-items: center;
      }

      .content-bar-middle {
        flex: 1;
        background-color: bisque;
        display: flex;
        align-items: center;
        flex-wrap: wrap;

        .bar-middle-item {
          width: 70px;
          background-color: gray;
          height: 30px;
          border-radius: 5px;
          margin-left: 10px;
          display: flex;
          align-items: center;
          justify-content: center;
        }
      }

      .content-bar-right {
        width: 20%;
        background-color: blueviolet;
        display: flex;
        align-items: center;
        flex-wrap: wrap;

        .content-bar-right-item {}
      }
    }
  }
}
</style>
