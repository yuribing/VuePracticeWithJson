<!--<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>
  <p>Edit <code>components/HelloWorld.vue</code> to test hot module replacement.</p>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      count: 0
    }
  }
}
</script>-->
<template>
  <div id="app">
    <ul>
      <li v-for="user in users" :key="user.id">
         {{user.name}}
       </li>
    </ul>
  </div>
</template>

<script>
import usersData from "/json/users.json";

export default {
  name: 'HelloWorld',
  data() {
    return {
      users: usersData,
    };
  },
};
</script>