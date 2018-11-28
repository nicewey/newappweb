<template>
  <div id="app">
    <!--这里会导致detail组建里的actived钩子失效-->
    <keep-alive exclude="Detail">
      <router-view/>
    </keep-alive>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>

</style>
