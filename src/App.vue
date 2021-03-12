<template>
  <div class="content">
    <div class="text">
      <div class="name"><span>Dane Erickson</span></div>
      <AboutList />
    </div>
    <div class="image">
      <img src='./assets/me.png' alt="me" />
    </div>
  </div>
</template>

<script>
import AboutList from './components/AboutList.vue'

export default {
  name: 'App',
  components: {
    AboutList
  }
}
</script>

<style>
body {
  color: #576366;
  background:rgb(15, 1, 53);
  margin: 0;
  font-family: 'Roboto', sans-serif;
}

.image {
  flex: 1;
  width: 25%;
}
.name {
  font-size: 5em;
  margin-left: -6px;
}
.content {
  color: white;
  display: flex;
  flex-direction: row;
  height: 100vh;
  overflow: auto;
  padding-left: 5em;
  padding-top: 5em;
  overflow: hidden;
}

.text {
  display: flex;
  flex-direction: column;
}
</style>
