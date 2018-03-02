<template>
  <div id="content">
    <v-header></v-header>
    <v-nav></v-nav>
    <div class="container">
      <keep-alive>
        <router-view/>
      </keep-alive>
    </div>
  </div>
</template>

<script>
import vHeader from 'com/vHeader/vHeader'
import vNav from 'com/vNav/vNav'
export default {
  name: 'content'
  , data() {
    return {
      
    }
  }
  , methods: {

  }
  , components: {
    vHeader
    ,vNav
  }
}
</script>

<style lang="stylus">
@import '../../assets/css/mixin'
#content,.container
  width 100%
  height 100%
  /*padding-top 56px
  padding-left 120px
  padding-bottom 30px
  overflow auto*/
</style>
