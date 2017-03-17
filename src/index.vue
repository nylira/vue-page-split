<template>
  <div class="ni-page-split">
    <div class="ni-page-split-header">
      <slot name="header"></slot>
    </div>
    <div class="ni-page-split-main">
      <slot name="main"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ni-page-split'
}
</script>

<style src="./style.css"></style>
