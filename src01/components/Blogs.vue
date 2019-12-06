<template>
  <div>
    <h2>河南省</h2>
    <ul>
      <Blog  v-for="(city, index) in citys" :key="city.id" :city1='city'/>
    </ul>
  </div>
</template>

<script type="text/ecmascript-6">
import Blog from './Blog'
  export default {
    data() {
      return {
        citys:[
          {id:1,name:'郑州'},
          {id:2,name:'洛阳'},
          {id:3,name:'开封'},
          {id:4,name:'安阳'},
          {id:5,name:'商丘'},
          {id:6,name:'信阳'}
        ]
      }
    },
    components:{
      Blog
    }
  }
</script>

<style scoped>

h2{
  color: red
}
</style>
