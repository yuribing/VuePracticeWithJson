<template>
<section>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld />
    <Member />
</section>
</template>

<script>
import Member from './components/Member.vue'

export default {
  name: 'app',
  components: {
    Member
  }
}
</script>
