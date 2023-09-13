<template>
  <h1>Job Details</h1>
  <p>The Job Id is {{ id }}</p>
</template>

<script>
export default {
  name: 'JobDetails',
  props:['id'],
  data() {
    return {
      //ids: this.$route.params.id,
    }
  },
}
</script>
