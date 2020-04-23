<template>
  <ul class="resource-list">
    <li class="resource-list-item" v-for="(item) in filteredResources" :key="item.id">
      <a :href="item.link" target="_blank">{{item.title}}</a>
    </li>
  </ul>
</template>

<script>
import resources from '@/data/resources.json'
export default {
  name: 'Resource-List',
  computed: {
    filteredResources () {
      return resources
    }
  } 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/styles/main.scss";
 ul {
    backface-visibility: hidden;
  }
  ul li {
    margin: 0 0 .6em;
    @include fluid-type(42px, 52px);
    text-transform: uppercase;
    letter-spacing: -.9px;
  }
</style>
