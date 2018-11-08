<template>
  <div class='container'>
    <div class="field has-addons">
    <div class='control has-icons-left is-expanded'>
      <input class='input is-medium' type='text' :placeholder='searchHint'>
      <span class='icon is-small is-left'>
        <i class='fas fa-search'></i>
      </span>
    </div>
    <div class='control'>
      <a class='button is-medium is-white far fa-times-circle fa-lg' v-on:click='searchApi'></a>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      searchHint: this.$constants.$SearchHint
    }
  },
  methods: {
    searchApi: function (event) {
      console.log('search APi Clicked.')
    }
  }
}
</script>

<style lang='scss' scoped>
  .input {
    border: 0;
    outline: none;
    border-radius: 0;
    box-shadow: none;
  }

  .button {
    border: 0;
    outline: none;
    border-radius: 0;
    box-shadow: none;
  }
</style>
