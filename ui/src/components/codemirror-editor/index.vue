<template>
  <Codemirror v-bind="$attrs" border :height="200" :option="cmOptions" />
</template>

<script setup lang="ts">
import Codemirror from 'codemirror-editor-vue3'

defineOptions({ name: 'CodemirrorEditor' })
const cmOptions = {
  mode: 'text/x-python',
  autoRefresh: true
}
</script>

<style lang="scss" scoped>
.codemirror-container.bordered {
  border: 1px solid #bbbfc4;
  border-radius: 4px;
}
.CodeMirror-gutters {
  left: 0 !important;
}
</style>
