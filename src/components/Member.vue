<template>

    <table border="1">
      <thead><td>ID</td><td>Name</td><td>Title</td></thead>
      <tbody>
        <tr v-for="user in users" :key="user.id">
          <td>{{user.id}}</td> 
          <td>{{user.name}}</td>  
          <td>{{user.title}}</td>  
        </tr> 
      </tbody>
    </table>

</template>

<script>
import usersData from "/json/users2.json";

export default {
  name: 'Member',
  data() {
    return {
      users: usersData,
    };
  },
};
</script>