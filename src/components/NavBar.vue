<template>    
  <nav>
    <router-link to="/" id="logo-url">
        <img :src="srcImage" :alt="altImage" id="logo">
    </router-link>
    <router-link to="/">Home</router-link>
    <router-link to="/pedidos">Pedidos</router-link>
  </nav>
</template>

<script>
export default {
    name: 'Navbar',
    props: [
      "srcImage",
      "altImage"
    ]
}
</script>

<style scoped>
nav {
  background-color: #222;
  border-bottom: 4px solid #111;
  padding: 15px 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

#logo-url{
  margin: auto;
  margin-left: 0;
}

#logo{
  height: 40px;
  width: 40px;
}

nav a{
  color: #FCBA03;
  text-decoration: none;
  margin: 12px;
  transition: .5s;
}

nav a:hover {
  color: #FFF;
}

</style>