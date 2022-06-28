<template>
  <div class="wrapper">
    <div class="container">
      <div class="dashboard">
        <img src="@/assets/Shape.svg" alt="">
        <span>Dashboard</span>
      </div>
      <h3>INVESTMENTS</h3>
      <h4>My Investments</h4>
      <h4>Short Term F.O.R.E.D</h4>
      <h4>Long Term F.O.R.E.D</h4>
      <h4>Permanent Ownership</h4>
    </div>
  </div>
</template>

<script>

export default {
  name: 'SideBar',
  components: {
}
}
</script>

<style scoped>
.wrapper {
  background: #FFFEE6;
  width: 20%;
  padding: 130px 30px;
}
.dashboard {
    padding-bottom: 37px;
}
.dashboard span {
    padding-left: 15px;
}
h3 {
    padding-bottom: 37px;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 24px;
    letter-spacing: 0.75px;
    color: #8A0C2C;
}
h4 {
    padding-bottom: 11px;
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 19px;
    color: #11142D;
}
</style>
