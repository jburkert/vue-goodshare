<template>
  <div>
    <vue-goodshare-facebook has_icon/>
    <vue-goodshare-linked-in has_icon/>
    <vue-goodshare-tumblr has_icon/>
    <vue-goodshare-twitter has_icon/>
  </div>
</template>

<script>
// Import VueGoodshare social network components
import VueGoodshareFacebook from "./providers/Facebook.vue";
import VueGoodshareTwitter from "./providers/Twitter.vue";
import VueGoodshareLinkedIn from "./providers/LinkedIn.vue";
import VueGoodshareTumblr from "./providers/Tumblr.vue";

export default {
  name: "VueGoodshare",
  components: {
    VueGoodshareFacebook,
    VueGoodshareLinkedIn,
    VueGoodshareTumblr,
    VueGoodshareTwitter
  }
};
</script>
