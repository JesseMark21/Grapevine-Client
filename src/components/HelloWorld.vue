<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Recipients</h2>
    <div id="input-container">
      <div>
        <!--element which is going to render the TextBox-->
        <input class="e-input" type="file" placeholder="Upload a CSV file" />
      </div>
    </div>

    <h2>Message</h2>
    <div id="input-container">
      <div>
        <!--element which is going to render the TextBox-->
        <input class="m-input" type="text" placeholder="Your Message Here"/>
      </div>
    </div>
    <h2>Personalisation</h2>
    <div class="e-float-input e-input-group">
            <input type="text" required/>
            <span class="e-float-line"></span>
            <label class="e-float-text"> Enter Personalised Values (as a comma separated list) Example: Name, Number </label>
        </div>
    <h2>Enable Service</h2>
    <input type="checkbox" id="sms" value="SMS Saver" v-model="checkedNames">
    <label for="sms">SMS Saver</label>
    <input type="checkbox" id="url" value="URL Shortening" v-model="checkedNames">
    <label for="url">URL Shortening</label>
    <!-- <ul>
      <li>
        <a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a>
      </li>
      <li>
        <a href="https://forum.vuejs.org" target="_blank" rel="noopener"
          >Forum</a
        >
      </li>
      <li>
        <a href="https://chat.vuejs.org" target="_blank" rel="noopener"
          >Community Chat</a
        >
      </li>
      <li>
        <a href="https://twitter.com/vuejs" target="_blank" rel="noopener"
          >Twitter</a
        >
      </li>
      <li>
        <a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a>
      </li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li>
        <a href="https://router.vuejs.org" target="_blank" rel="noopener"
          >vue-router</a
        >
      </li>
      <li>
        <a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-devtools#vue-devtools"
          target="_blank"
          rel="noopener"
          >vue-devtools</a
        >
      </li>
      <li>
        <a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener"
          >vue-loader</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/awesome-vue"
          target="_blank"
          rel="noopener"
          >awesome-vue</a
        >
      </li>
    </ul> -->
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
h2 {
  margin: 20px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.m-input {
  width: 800px;
  height: 200px;
  margin: 0 0 0;
}
a {
  color: #42b983;
}
</style>
