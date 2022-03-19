<template>
  <div class="dest">
    <h1 class="dest__title"><span>01</span>Pick your destination</h1>
  </div>
</template>

<style lang="scss" scoped>
.dest {
  height: 100vh;
  background: url('../assets/destination-bg-m.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  padding-top: 88px;

  &__title {
    font-size: 20px;
    text-transform: uppercase;
    text-align: center;
    color: #fff;
    letter-spacing: 3px;
  }

  &__title span {
    opacity: 25%;
    display: inline-block;
    margin-right: 18px;

  }
}
</style>