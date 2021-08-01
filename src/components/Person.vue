<template>
  <div id="Person" @mouseenter="over = !over" @mouseleave="over = !over" >
    <div id="ProfilePicture">
    </div>
    <div id="TextArea">
      <div>
        <h4>Ipson Lorem ipsum dolor</h4>
        <p>sit amet, consectetur adipisicing elit.</p>
      </div>
    </div>
    <div id="TimeArea">
      6:53 PM
      <button id="arrow" v-if="over">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path d="M0 7.33l2.829-2.83 9.175 9.339 9.167-9.339 2.829 2.83-11.996 12.17z"/>
        </svg>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data: function(){
    return{
      over: false,
    }
  },
}
</script>

<style>
#Person{
  width: 30vw;
  height: 13%;
  background-color: #131c21;
  color: #abbcb8;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  border-top: 1px solid #192126;
  border-width: 15%;
}
#Person:last-child{
  border-bottom: 1px solid #192126;
}
#Person:hover{
  background-color: #282c2e;
}

p{
  font-size: 14px;
}
#ProfilePicture{
  height: 49px;
  width: 49px;
  background-color: slateblue;
  border-radius: 50%;
}

#TextArea{
  width: 60%;
}
#TimeArea{
  margin-top: 5%;
  display: flex;
  flex-direction: column;
  font-size: 13.5px;
  align-self: flex-start;
}

@keyframes showUp {
  0%{
    opacity: 0;
    transform: translateX(20px);
  }
  100%{
    opacity: 1;
    transform: translateX(0);
  }
}

#arrow{
  align-self: flex-end;
  fill: #abbcb8;
  cursor: pointer;
  background-color: #282c2e;
  animation: showUp linear 0.1s;
}

</style>