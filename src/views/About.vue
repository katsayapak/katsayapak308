<template>
  <div class="about">
    <h1>This is an about page</h1>
    
  </div>
</template>
 <script>
export default {
  data() {
    return {
      users: []
    };
  },
  mounted() {
    axios
      .get("https://vue-js-1a60d.firebaseio.com/")
      .then(response => {
        console.log(response);
        const data = response.data;
        for (let key in data) {
          const user = data[key];
          user.id = key;
          this.users.push(user);
        }
      })
      .catch(error => {
        console.log(error);
      });
  }
};
</script>
 