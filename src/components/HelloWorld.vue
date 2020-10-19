<template>
<div class= "header-container">
    <h1 @click="onClickTitle">{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      titleclassname : '',
    }
  },
  props: {
    msg: String
  },
  methods: {
    onClickTitle(){
      this.titleclassname= "header-container header"
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
//@import "../styles/components/header.scss";
$container-width: 90%;

.header-container {
  width: $container-width;
  height: 100vh;
  font-size: 100px;
  background-color: cornflowerblue;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: bold;
  transition: all 0.4s linear;
  :hover {
    color: black;
    animation: header 1s linear;
  }
}

@keyframes header {
  0% {
    transform: scaleX(1);
  }
  50% {
    transform: scaleX(0.5);
  }
  100% {
    transform: scaleX(0.2);
  }
}

</style>