<template>
  <div id="PersonContainer">
    <HeaderProfile/>
    <Searcher/>
    <div id="Container">
      <Person/>
      <Person/>
      <Person/>
      <Person/>
      <Person/>
      <Person/>
      <Person/>
      <Person/>
      <Person/>
      <Person/>
      <Person/>
    </div>
  </div>
</template>

<script>
import Person from '../components/Person.vue'
import HeaderProfile from './HeaderProfile.vue'
import Searcher from './Searcher.vue'

export default {
  components: { Person, HeaderProfile, Searcher },
}
</script>

<style>
  #PersonContainer{
    width: 30vw;
    height: 100vh;
  }

  #Container{
    height: 100%;
    overflow-y: scroll;
  }
  #Container::-webkit-scrollbar{
    width: 5px;
    background-color: #131c21;
  }
  #Container::-webkit-scrollbar-thumb{
    background-color: #394045;
    
  }

</style>