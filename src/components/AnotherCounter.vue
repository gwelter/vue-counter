<template>
    <div>
        <button class="btn btn-primary" @click="increment(100)">Another Increment by 100</button>
        <button class="btn btn-primary" @click="asyncDecrement({by: 50, duration: 500})">Another asyncDecrement</button>
    </div>
</template>

<script>
  import { mapActions } from 'vuex'
  export default {
    methods: {
      ...mapActions([
        'increment',
        'asyncDecrement'
      ])
    }
  }
</script>