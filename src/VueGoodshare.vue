<template>
  <div>
    <div v-if="this.$props.bundle === 'world'">
      <vue-goodshare-facebook has_icon has_counter title_social="Facebook"/>
      <vue-goodshare-linked-in has_icon has_counter title_social="LinkedIn"/>
      <vue-goodshare-tumblr has_icon has_counter title_social="Tumblr"/>
      <vue-goodshare-twitter has_icon title_social="Twitter"/>
    </div>
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
  props: {
    bundle: {
      type: String,
      default: "world"
    }
  },
  components: {
    VueGoodshareFacebook,
    VueGoodshareLinkedIn,
    VueGoodshareTumblr,
    VueGoodshareTwitter
  }
};
</script>
