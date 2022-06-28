<template>
  <div class="container">
    <!-- Sidebar -->
    <side-bar />

    <!-- Page Content -->
    <div class="page-content">

      <!-- Header Bar -->
      <div class="header-bar">
        <img src="@/assets/check.svg" alt="" >
        <div class="right">
          <v-badge content="4">
            <img src="@/assets/notification.svg" alt="">
          </v-badge>
          <div class="account">
            <h1>John Doe</h1>
            <p>Account</p>
          </div>
          <v-badge
          bottom
          color="green"
          dot
          offset-x="10"
          offset-y="10"
          >
            <v-avatar size="40">
              <v-img src="@/assets/profile-pic.png"></v-img>
            </v-avatar>
          </v-badge>
        </div>
      </div>

      <!-- Heading -->
      <h1 class="heading">JASPER SMART CITY, IBEJU-LEKKI | 5-Bedroom Terrace Duplex</h1>

      <!-- Gallery -->
      <div class="gallery-container">
        <h3>Gallery</h3>
        <div class="gallery">
          <img src="@/assets/house1.png" alt="">
          <img src="@/assets/house2.png" alt="">
          <img src="@/assets/house3.png" alt="">
          <img src="@/assets/house4.png" alt="" class="last">
        </div>
      </div>

      <!-- Overview -->
      <div class="overview-container">
        <img src="@/assets/house3.png" alt="" class="video">
        <div class="overview">
          <p>Overview</p>
          <div class="chart-container">
            <ul>
              <li>5-Bedroom Terrace Duplex</li>
              <li>30 Blocks Available</li>
              <li>Fractionalized into 15 Slots Per Block</li>
              <li>Total Slots Available: 450 Slots</li>
            </ul>
            <div class="chart">
              <img src="@/assets/chart.svg" alt="">
            </div>
          </div>
        </div>
      </div>

      <!-- Purchase Section -->
      <div class="purchase-container">
        <div class="buy-as-group">
          <div class="title">
            <p>Buy as a Group</p>
          </div>
          <p class="description">Buy as a group and divide a unit between family and friends. You are automatically made a moderator of the group. You can add group members by their email address. Group members can be a Gvest member or anyone with a valid email address.</p>
          <div class="title"></div>
          <div class="title">
            <p>Group Members</p>
            <button><img src="@/assets/+.svg" alt=""> Add Member</button>
          </div>
          <div class="customer-container">
            <div class="customers">
              <div class="email">
                <h3>Customer/Email</h3>
                <input type="email" name="email" />
                <p class="total">Amount to pay = ₦31,666,666.67</p>
              </div>
              <div class="ratio"></div>
            </div>
            <button class="continue">Continue</button>
          </div>
        </div>
        <div class="buy-as-unit">
          <div class="title">
            <p>Buy Fractional Unit</p>
          </div>
          <p class="description">Buy a fractional unit of a property in this estate, each property allows 15 slots. To buy a complete property, you can buy 15 slots. <br> <br> How may slots do you want to buy?</p>
          <div class="title">
            <p>1</p>
          </div>
          <p class="total">Total value = ₦6,333,333.33</p>
          <button class="continue">Continue</button>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
import SideBar from '@/components/SideBar.vue'

export default {
  name: 'App',
  components: {
    SideBar
}
}
</script>

<style scoped>
.container {
  display: flex;
  width: 100%;
}
.page-content {
  display: flex;
  flex-direction: column;
  padding: 10px 20px;
  width: 80%;
}
.header-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-radius: 6px;
  box-shadow: 0px 4px 24px rgba(0, 0, 0, 0.12);
  margin-bottom: 55px;
}
.header-bar img {
  padding: 20px;
}
.account {
  padding-right: 14px;
}
.account h1 {
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 21px;
  text-align: right;
  color: #6E6B7B;
}
.account p {
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: right;
  color: #B9B9C3;
}
.right {
  display: flex;
  align-items: center;
}

.heading {
  font-style: normal;
  font-weight: 600;
  font-size: 32px;
  line-height: 24px;
  letter-spacing: 0.75px;
  color: #8A0C2C;
  padding-bottom: 32px;
}

.gallery-container h3 {
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 22px;
  color: #11142D;
  padding-bottom: 14px;
}
.gallery {
  justify-content: space-between;
  padding-bottom: 23px;
}
.gallery img {
  width: 25%;
  padding-right: 21px;
}
.gallery .last {
  padding-right: 0;
  padding-top: 40px;
}

.overview-container {
  display: flex;
  border-radius: 5px;
}
.video {
  width: 50%;
  height: 278px;
  padding-right: 18px;
}
.overview {
  background: #FFFEE6;
  padding: 36px 20px;
  width: 50%;
}
.overview p {
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 22px;
  color: #000000;
  padding-bottom: 22px;
}
ul {
  list-style: none;
  padding: 0 35px;
  width: 80%;
}
ul li::before {
  content: "\2022";  /* Add content: \2022 is the CSS Code/unicode for a bullet */
  color: red; /* Change the color */
  font-weight: 900; /* If you want it to be bold */
  display: inline-block; /* Needed to add space between the bullet and the text */
  width: 1em; /* Also needed for space (tweak if needed) */
  margin-left: -1em; /* Also needed for space (tweak if needed) */
}
li {
  padding-bottom: 20px;
}
.overview img {
  margin-top: -20px;
}
.chart-container {
  display: flex;
}

.purchase-container {
  display: flex;
  padding-top: 24px;
}
.title {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: rgba(243, 242, 247, 0.7);
  padding: 17px 8px;
  margin-bottom: 15px;
}
.title p {
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.75px;
  color: #1C1939;
}
.buy-as-group {
  width: 50%;
  padding-right: 25px;
}
.buy-as-unit {
  width: 50%;
}
.description {
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.75px;
  color: #706666;
  padding: 0 9px;
}
.total {
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 24px;
  letter-spacing: 0.75px;
  color: #17A2B8;
}
button {
  background: #8A0C2C;
  border-radius: 5px;
  padding: 8px 22px;
  color: #ffffff;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.75px;
}
.continue {
  width: 100%;
}
.customer-container {
  border: 1px solid #CECDD2;
  border-radius: 5px;
  padding-top: 16px;
  padding-left: 21px;
  padding-right: 21px;
}
</style>
