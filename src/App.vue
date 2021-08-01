<template>
  <div id="app">
    <PersonContainer/>
    <ChatContainer/>
  </div>
</template>

<script>
import ChatContainer from './components/ChatContainer.vue'
import PersonContainer from './components/PersonContainer.vue'

export default {
  components: { ChatContainer, PersonContainer }
}
</script>

<style>
    *{
        padding: 0;
        margin: 0;
        vertical-align: baseline;
        border: 0;
    }
    body{
        height: 100%;
        width: 100%;
    }
    #app{
      display: flex;
      justify-content: space-between;
      overflow-y: hidden;
    }
</style>