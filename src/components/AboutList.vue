<template>
  <div class="listItem" v-for="item in listItems" :key="item.value">
    <span v-if="!item.onClick">
      {{ item.value }}
    </span>
    <span class="linkText" v-else @click="item.onClick">
      {{ item.value }}
    </span>
  </div>
</template>
<script>
import listItems from '../assets/list'

export default {

  data() {
    return {
      listItems
    }
  },
}
</script>

<style>
.linkText:hover {
  cursor: pointer;
  text-decoration: underline;
}
.listItem {
  padding-top: 1em;
}
</style>
