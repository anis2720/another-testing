<template>
  <div class="footer">
    <div class="left">Portfolio by <router-link to="/resume"> AnisH</router-link></div>
    <div class="right">Reach me at <a href="mailto:my@email.com">anishadi.1412@gmail.com</a> or <router-link to="/contact">through here</router-link></div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Footer"
});
</script>

<style scoped lang="less">

@import '../css/variables.less';

a {
  color:	#2ECC71;
  text-decoration: none;
  opacity: 1;
}
a:hover, .router-link-exact-active {
  color:	#2ECC71;
  font-weight: bold;
  text-decoration: underline;
  opacity: 1;
}


.footer {
  background-color: @bodyBgColor;
  width: 100%;
  font-size: 0.8em;
  opacity: 0.7;
  padding-bottom: 30px;
}

.left, .right {
    padding-top: 10px;
    text-align: center;
  }

@media only screen and (min-width: 620px){

  .footer {
    padding: 0;
    color: #ffffff;
  }

  .left, .right {
    padding: 20px;
  }

  .left {
    float: left;
  }

  .right {
    float:right;
  }
}
</style>