<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Fill in all the fields and I will create a silly MadLibs for you!
    </p>
    <form>

    </form>
  </div>
</template>

<script>
import axios from 'axios';
export default {
  name: 'HelloWorld',
  mounted()
  {
    axios.get('https://api.sampleapis.com/wines/reds').then((resp) => {
      console.log(resp);
    })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
