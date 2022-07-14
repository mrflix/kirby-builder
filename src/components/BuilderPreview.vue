<template>
  <div class="kBuilderPreview">
    <div id="kirby-builder-content" v-html="markup"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      previewFrameWindow: {},
      previewFrameDocument: {},
      previewHeight: 0
    };
  },
  props: {
    markup: {
      type: String
    },
    styles: {
      type: String
    },
    script: {
      type: String
    },
    cssContent: {
      type: String
    },
    index: {
      type: Number
    }
  }
};
</script>
