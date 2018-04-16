<template>
  <div>
    <p>Double counter is: {{ dobleCounter }}</p>
    {{stringCounter}}
  </div>
</template>

<script>
  import { mapGetters } from 'vuex'
  export default {
      computed: {
        ...mapGetters([
          'dobleCounter',
          'stringCounter'
        ])
      }
  }
</script>