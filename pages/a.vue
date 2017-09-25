<template>
  <div>
    <div style="border:1px dashed #dedede; padding: 10px;">
      <ul>
        <li><nuxt-link to="/a/">Go to /a/</nuxt-link></li>
        <li><nuxt-link to="/a/b/">Go to /a/b/</nuxt-link></li>
        <li><nuxt-link to="/a/c/">Go to /a/c/</nuxt-link></li>
      </ul>
    </div>
    <div style="border:1px dashed #dedede; padding: 10px;">
      <nuxt-child/>
    </div>
  </div>
</template>

<script>
export default {
  created () {
    console.log('a created')
  },
  beforeDestroy () {
    console.log('a is about to be destroyed')
  }
}
</script>
