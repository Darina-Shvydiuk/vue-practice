<template>
<div class="search flex">
<input type="text" class="search" v-model="searchText"/>
<button type="button" @click="$emit('search',searchText)">Search</button>
</div>
</template>
<script>
export default {
  name: 'SearchGoods',
  data () {
    return {
      searchText: ''
    }
  }
}
</script>
<style lang="scss" scoped>
input {
  height: 25px;
  margin-left: 40px;
}
button {
  background-color: rgb(221, 56, 56);
  color: #fff;
  border: none;
  border-radius: 4px;
  padding: 8px 14px;
  display: block;
  cursor: pointer;
  margin-left: 10px;
}
</style>
