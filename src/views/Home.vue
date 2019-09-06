<template>
  <div class="home">
    <h1>Hello</h1>
    {{ loggedIn }}
  </div>
</template>

<script>
import { mapGetters } from 'vuex';

export default {
  name: 'home',
  computed: {
    ...mapGetters('auth', [
      'loggedIn'
    ])
  },
}
</script>
