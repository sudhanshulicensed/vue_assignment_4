<template>
  <div id="app">
    <CardTemplate>
      <div class="header" slot="header">
        <img src="https://picsum.photos/600/300/?image=25" alt="Card Image">
      </div>
      <div class="title" slot="title">
        <h1 class="para">Card Title</h1>
      </div>
      <div class="body" slot="body">
        <p class="para">Some quick example text to build on the card title and make up the bulk of the card content.</p>
      </div>
      <div class="footer" slot="footer">
        <button class="button">{{ text }}</button>
      </div>
    </CardTemplate>
  </div>
</template>

<script>

import CardTemplate from "./components/Card.vue"

export default {
  name: 'App',
  components: {
    CardTemplate
  },
  data() {
    return {
      text: "Go Somewhere"
    }
  }
}
</script>

<style>
  #app{
    font-family: sans-serif;
    width: 250px;
    height: 280px;
    margin-top: 100px;
    margin-left: auto;
    margin-right: auto;
    border: 1px solid #bdc3c7;
  }

  .header{
    height: 30%;
  }

  .header img{
    width: 100%;
    height: 100%;
  }

  .title{
    width: 90%;
    margin-left: auto;
    margin-right: auto;
  }

  .body{
    height: 25%;
    width: 90%;
    margin-left: auto;
    margin-right: auto;
  }

  .body p{
    color: #2d3436;
    font-size: 12px;
    line-height: 1.6;
  }

  .para{
    font-size: 16px;
    font-weight: 400;
  }

  .footer{
    height: 40%;
    width: 90%;
    margin-left: auto;
    margin-right: auto;
  }

  .button{
    width: 100px;
    box-sizing: border-box;
    padding: 2%;
    background-color: #007BFF;
    color: #fff;
    border-radius: 3px;
    border: 1px solid #007BFF;
    font-size: 12px;
}



</style>
