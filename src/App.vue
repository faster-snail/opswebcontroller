<template>
    <div>
      <Bar/>
      <div class="bottom-main">
        <List class="my-list elevation-0"/>
        <v-content>
          <HelloWorld/>
        </v-content>
      </div>
      
    </div>
   
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Bar from './components/Bar'
import List from './components/List'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Bar,
    List
  },
  data () {
    return {
      //
    }
  }
}
</script>
<style>
.my-list {
  height: 100vh;
  width: 20%;
  float: left;
}
.v-content {
  float: right;
  width: 80%;
  height: 100vh;
}
.bottom-main {
  margin-top: 5px;
}

</style>
