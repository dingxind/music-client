<template>
  <div class="the-footer">
    <p v-for="(item, index) in list" :key="index">
    {{item}}
    </p>
     <el-link href="https://blog.csdn.net/qq_17589751"  target="_blank">Designed by Xindong</el-link>
  </div>
</template>

<script>
export default {
  name: 'the-footer',
  data () {
    return {
      list: [
        `关于 | 帮助 | 条款 | 反馈`,
        `Copyright © 2020`,
      ]
    }
  }
}
</script>

<style scoped>
.the-footer{
  width: 100%;
  background-color: #81D5EF;
  height: 200px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.the-footer p {
  height: 25px;
}
</style>
