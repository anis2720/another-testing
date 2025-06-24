<template>
  <div class="footer">
    <div class="left">Portfolio by AnisH</div>
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

.footer {
  background-color: @bodyBgColor;
  width: 100%;
  font-size: 0.8em;
  opacity: 1;
  padding-bottom: 30px;
  color:#cbd7e1;
}

.footer a {
  color:#FFD966; // Soft yellow
  text-decoration: underline;
}

.footer a:hover {
  color: #cbd7e1;
}

.left, .right {
  padding-top: 10px;
  text-align: center;
}


@media only screen and (min-width: 620px){

  .footer {
    padding: 0;
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