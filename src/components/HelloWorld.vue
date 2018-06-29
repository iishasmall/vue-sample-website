<template>
  <div class="hello">
    <div class="slanted">
    <h2>Hello World!</h2>
   <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perspiciatis et debitis pariatur perferendis adipisci doloribus aspernatur ea quo illum a.</p>
    </div>
    <div class="slanted">
    <h2>Hello World!</h2>
   <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perspiciatis et debitis pariatur perferendis adipisci doloribus aspernatur ea quo illum a.
   Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perspiciatis et debitis pariatur perferendis adipisci doloribus aspernatur ea quo illum a.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.box-shadow {
 box-shadow: inset 0 0 10px #000000;
}

.slanted {
    background: linear-gradient(15deg,#ccc,#fff);
    margin: 0 auto;
    box-sizing: border-box;
    width: 100%;
    position: relative;
    padding: 20px;
    clip-path: polygon(0% 0%, 100% 100%, 100% 85%, 0 100%);
    -webkit-clip-path: polygon(0% 0%, 100% 20%, 100% 100%, 0 100%);
}

.slanted:before {
    content: "";
    background: #00;
    height: 40px;
    transform: skewY(2deg);
    position: absolute;
    left: 0;
    right: 0;
    z-index: -1;
}

.slanted:after {
    content: "";
    background: #fff;
    height: 40px;
    transform: skewY(1deg);
    position: absolute;
    left: 0;
    right: 0;
    z-index: -1;
}

.slanted:before{
    top: -20px;

}

.slanted:after {
    bottom: -30px;
}
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
