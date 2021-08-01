<template>
  <div id="ChatHeader">
    <div id="ChatContainerText">
      <div id="FriendPhoto"/>
      <div id="TextChat">
        <h4>Nome</h4>
        <p>visto por último .......</p>
      </div>
    </div>
    <div id="ButtonsChatContainer">
      <div class="ButtonsChat">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
          <path fill="currentColor" d="M15.9 14.3H15l-.3-.3c1-1.1 1.6-2.7 1.6-4.3 0-3.7-3-6.7-6.7-6.7S3 6 3 9.7s3 6.7 6.7 6.7c1.6 0 3.2-.6 4.3-1.6l.3.3v.8l5.1 5.1 1.5-1.5-5-5.2zm-6.2 0c-2.6 0-4.6-2.1-4.6-4.6s2.1-4.6 4.6-4.6 4.6 2.1 4.6 4.6-2 4.6-4.6 4.6z"></path>
        </svg>
      </div>
      <div class="ButtonsChat">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
          <path fill="currentColor" d="M12 7a2 2 0 1 0-.001-4.001A2 2 0 0 0 12 7zm0 2a2 2 0 1 0-.001 3.999A2 2 0 0 0 12 9zm0 6a2 2 0 1 0-.001 3.999A2 2 0 0 0 12 15z"></path>
        </svg>
      </div> 
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
#ChatHeader{
  width: 100%;
  height: 59px;
  background-color: #2a2f32;
  border-left: 1px solid #192126;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
#FriendPhoto{
    background-color: indigo;
    border-radius: 50%;
    width: 40px;
    height: 40px;
}
.ButtonsChat{
  height: 40px;
  width: 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  color: #b1b3b5;
  cursor: pointer;
  }
.ButtonsChat:active{
  background-color: #272a2c;
}
#ButtonsChatContainer{
  margin-right: 3%;
  display: flex;
  align-items: center;
}
#ChatContainerText{
  margin-left: 1%;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  width: 20%;
  color: #c7c9ca;
}

</style>