<template>
  <div class="home">
    <ResourceList />
  </div>
</template>

<script>
// @ is an alias to /src
import ResourceList from '@/components/ResourceList.vue'

export default {
  name: 'Home',
  components: {
    ResourceList
  }
}
</script>
