<template>
  <div id="ChatContainer">
  <HeaderChat/>
  <Chat/>
  <InputChat/>
  </div>
</template>

<script>
import HeaderChat from './HeaderChat.vue'
import Chat from './Chat.vue'
import InputChat from './InputChat.vue'

export default {
  components:{ HeaderChat, Chat, InputChat }
}
</script>

<style>
  #ChatContainer{
    background-image: url('../assets/bg.jpg');
    width: 70vw;
    overflow: hidden;
    background-size: contain;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

</style>