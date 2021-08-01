<template>
  <div id="Searcher">
    <button id="search" v-if="!focused">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
        <path fill="currentColor" d="M15.009 13.805h-.636l-.22-.219a5.184 5.184 0 0 0 1.256-3.386 5.207 5.207 0 1 0-5.207 5.208 5.183 5.183 0 0 0 3.385-1.255l.221.22v.635l4.004 3.999 1.194-1.195-3.997-4.007zm-4.808 0a3.605 3.605 0 1 1 0-7.21 3.605 3.605 0 0 1 0 7.21z"></path>
      </svg>
    </button>
    <button id="back" v-if="focused">
      <svg width="24" height="24" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd" id="svg">
        <path d="M21.883 12l-7.527 6.235.644.765 9-7.521-9-7.479-.645.764 7.529 6.236h-21.884v1h21.883z"/>
      </svg>
    </button>
    <input type="text" placeholder="Pesquisar ou começar uma nova conversa" @focus="invert" @blur="invert">
    <button id="close">

    </button>
  </div>
</template>

<script>
export default {
  data: function(){
    return{
      focused:false
    }
  },
  methods: {
    invert(){
      this.focused = !this.focused
    }
  }
}
</script>

<style>
  #Searcher{
    width: 100%;
    height: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #131c21;
    border-bottom: 1px solid #192126;
    border-right: 1px solid #192126;

  }
  input{
    font-size: 14px;
    width: 65%;
    height: 72%;
    background-color: #323739;
    color: #787b7c;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0px 20px 0px 20px ;
  }
  input:focus{
    outline: none;
  }
  #search{
    border-radius: 20px 0 0 20px;
    width: 40px;
    height: 72%;
    background-color: #323739;
    cursor: pointer;
    color: #787b7c;
  }
  #close{
    border-radius: 0 20px 20px 0;
    width: 40px;
    height: 72%;
    background-color: #323739;
  }

  #back{
    border-radius: 20px 0 0 20px;
    width: 40px;
    height: 72%;
    background-color: #323739;
    cursor: pointer;
    fill:#787b7c;
  }

  @keyframes rotation{
    100%{
      transform: rotate(180deg);
    }
  }
  #svg{
    animation: rotation linear 0.3s;
    animation-fill-mode: forwards;
  }

</style>

