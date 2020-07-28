<template>
  <div>
    <span>{{ title }}</span>
  </div>
</template>
<script>
export default {
  data() {
    return {
      title: ''
    }
  },
  mounted() {
    console.debug(this.$route.name)
    this.$route.meta.title = 'test'

    if (this.$route.params.title) {
      this.title = this.$route.params.title
    }
  },
  methods: {
  }
}
</script>>
