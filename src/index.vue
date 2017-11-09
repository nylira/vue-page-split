<template>
  <div class="ni-page-split">
    <div class="ni-page-split-header">
      <slot name="header"></slot>
    </div>
    <div class="ni-page-split-main">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ni-page-split'
}
</script>

<style lang="stylus">
@require '~@/styles/variables.styl'

.ni-page-split
   min-height 75vh
   display flex
   flex-flow column nowrap

.ni-page-split-main
   flex 1
   background app-bg

@media screen and (min-width: 1024px)
   .ni-page-split
      flex-flow row nowrap
      align-items stretch
   .ni-page-split-header
      flex 0 0 33.3vw
      margin-bottom 0
      border-bottom none
   .ni-page-split-main
      flex 0 0 66.7vw

@media screen and (min-width: 1280px)
   .ni-page-split-header
      flex 0 0 25vw
   .ni-page-split-main
      flex 0 0 75vw
</style>
