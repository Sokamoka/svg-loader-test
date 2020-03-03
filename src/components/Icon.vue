<template>
  <div class="icons">
    <component :is="componentFile" v-bind="$attrs" ref="icon"></component>
  </div>
</template>
<script>
export default {
  name: "Icon",

  inheritAttrs: false,

  props: {
    name: {
      type: String,
      required: true
    }
  },

  mounted() {
    console.log("refs:", this.$refs);
  },

  computed: {
    componentFile() {
      console.log("name:", this.name);
      return () => import(`@/assets/${this.name}.svg`);
    }
  }
};
</script>
