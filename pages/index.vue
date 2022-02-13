<template>
  <div>
    <div class="background" ></div>
    <div class="container" >
      <h2>Bienvenidos a la app de Pokemons!</h2>
      <p>
        aquí encontrarás algunos de tus pokemons favoritos
      </p>
      <nuxt-link to="/Principal">
        <button class="button">Quiero ver!</button>
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
};
</script>

<style>

  .background {
    width: 100vw;
    height: 100vh;
    background: no-repeat;
    background-size: cover;
    background-image: url("https://cronicaglobal.elespanol.com/uploads/s1/41/84/43/3/pokemon-2.jpeg");
  }

  .container {
    position: absolute;
    top: 10vh;
    left: 10vw;
    width: 80vw;
    height: 80vh;
    background: no-repeat;
    background-size: cover;
    background-color: rgba(44, 44, 44, 0.671);
    backdrop-filter: blur(5px);
    margin: 0px;
    border-radius: 50px;
  }

  .container h2 {
    text-align: center;
    color: white;
    text-shadow: 1px 1px 2px black;
    margin: 0px;
    padding-top: 140px;
    font-size: 50px;
}

.container p {
    text-align: center;
    color: white;
    text-shadow: 1px 1px 2px black;
    font-size: 20px;
    text-transform: uppercase;
}

.button {
    position: absolute;
    bottom: 50px;
    margin-bottom: 50px;
    left: calc(50% - 125px);
    color: rgb(255, 255, 255);
    text-shadow: .5px .5px 2px black;
    width: 250px;
    height: 50px;
    border-radius: 10px;
    border: 3px solid rgba(223, 223, 223, 0.582);
    font-size: 20px;
    background-color: rgba(255, 255, 255, 0.411);
    backdrop-filter: blur(10px);
    box-shadow: 3px 3px 5px black;
    transition: all .3s;
}

.button:hover {
    color: rgb(51, 51, 51);
    border-radius: 30px;
    width: 200px;
    border: 3px solid rgb(128, 128, 128);
    left: calc(50% - 100px);
    height: 55px;
    background-color: rgba(255, 255, 255, 0.774);
}


</style>
