<template>
  <p class="demo">
    from break: {{ title || 'default' }}
  </p>
</template>

<script>
  export default {
    props: {
      title: { default: 'default title' }
    },
    data () {
      return {
        msg: 'Hello this is <Foo-Bar>'
      }
    }
  }
</script>
