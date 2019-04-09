<template>
  <div class="tick" @scroll="onScroll">
    <div class="dummy" ref="dummy" :style="dummyStyle"/>
    <div class="tick-inner" ref="tick-inner">
      <slot/>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'TickScroll',
  data() {
    return {
      dummy: {
        height: 0,
      },
    };
  },
  props: ['tick'],
  computed: {
    dummyStyle(): any {
      return {
        height: this.dummy.height + 'px',
      };
    },
  },
  methods: {
    onScroll() {
      return;
    },
  },
  mounted() {
    const el = this.$refs['tick-inner'] as HTMLElement;
    this.dummy.height = el.offsetHeight;
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.tick {
  position: relative;
  overflow: scroll;
}
.tick-inner {
  position: fixed;
  top: 0;
  left: 0;
}
</style>
