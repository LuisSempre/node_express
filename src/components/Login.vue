<template>
  <div>
    <h2>Login</h2>
    <form @submit.prevent="login">
      <input v-model="username" type="text" placeholder="Username" />
      <input v-model="password" type="password" placeholder="Password" />
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: '',
      password: ''
    };
  },
  methods: {
    login() {
      // Simulate authentication (replace this with your actual login logic)
      if (this.username === 'user' && this.password === 'password') {
        this.$router.push('/about'); // Redirect to the main app page
      } else {
        alert('Invalid credentials');
      }
    }
  }
};
</script>

