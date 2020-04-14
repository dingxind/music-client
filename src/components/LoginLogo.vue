<template>
  <div class="login-logo">
    <div class="item-logo">
      <svg class="icon" aria-hidden="true">
        <use xlink:href="#icon-yinle-"></use>
      </svg>
    </div>
  </div>
</template>

<script>
export default {
  name: 'login-logo'
}
</script>

<style scoped>
.login-logo{
  background-color: #2aa3ef;
  height: 100vh;
  width: 45%;
  overflow: hidden;
}
.item-logo {
  transform: rotate(-30deg);
}
.icon {
  width: 700px;
  height: 700px;
  fill: currentColor;
  color: #2796dd;
}
</style>
