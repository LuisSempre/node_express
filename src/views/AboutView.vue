<template>
  <div class="about">
    <h1>This is an about page</h1>
		    <button @click="logout">Logout</button>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>

<script>
export default {
  methods: {
    logout() {
      // Coloque aqui a lógica de logout
      // Por exemplo, redirecionar para a página de login
      this.$router.push('/');
    }
  }
};
</script>
