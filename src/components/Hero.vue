<template>
    <section class="hero">
        <div id="myHero" class="hero-body">
            <div class='container'>
                <h1 class="title">
                    {{ appName }}
                </h1>
                <Search />
            </div>
        </div>
    </section>
</template>

<script>
// https://vuejs.org/v2/guide/single-file-components.html
import Search from './Search'

export default {
  name: 'Hero',
  components: {
    Search
  },
  data () {
    return {
      appName: this.$constants.$AppName
    }
  }
}
</script>

<style lang='scss'>
@import "../main.scss";

.title {
  font-size: $size-extra-extra-large;
  font-weight: $weight-extra-light;
  @include mobile {
    font-size: $size-extra-large;
  }
}
</style>
