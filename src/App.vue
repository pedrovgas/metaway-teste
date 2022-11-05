<template>
  <nav>
    <span class="material-icons">
      menu
    </span>
    <router-link to="/">Home</router-link>
    <router-link to="/">Teste</router-link>
    <router-link to="/about">About</router-link>
  </nav>
  <router-view />

</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

nav {
  border-radius: 320px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 75px;
  position: fixed;
  background-color: #2c3e50;
  width: 75px;
  overflow: hidden;
  margin: auto;
  bottom: 0px;
  left: 50%;
  transform: translate(-50%, -50%);
  transition: width 200ms;
  transition-timing-function: ease-in-out;
  transition: 500ms;
  opacity: .5;

  &:hover {
    width: 15vw;
    opacity: 1;
  }

  &:hover a {
    display: block;
  }

  &:hover span{
    display: none;
  }
}

nav a {
  transition: 500ms;
  color: white;
  text-decoration: none;
  display:none
}

nav span.material-icons{
  color: white;
  font-size: 30px;
}
</style>
