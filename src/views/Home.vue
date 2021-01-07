<template>
  <div class="home">
    <div class="top-section">
      <div class="input-container">
        <input
          type="text"
          placeholder="Ingresa el nombre del Pokemon..."
          class="search"
        />
      </div>
    </div>
    <main class="main">
      <div class="pokemon-list">
        <section class="pokemon-container">
          <div class="poke-basic-info">
            <h3>Nombre</h3>
            <div class="basic-power">
              <span>power 1</span>
              <span>power 2</span>
            </div>
          </div>
          <div class="poke-image">image</div>
        </section>
      </div>
    </main>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
};
</script>
<style>
.top-section {
  height: 15rem;
  background-color: var(--light-red);
  display: flex;
  justify-content: center;
  align-items: center;
  border-bottom: 0.4rem solid var(--black);
}
.input-container {
  background-color: var(--bg-color);
  justify-content: center;
  align-items: center;
  display: flex;
  width: 30%;
  height: 5rem;
  border-radius: 100px;
  position: relative;
  top: 7.5rem;
  transition: box-shadow 0.2s;
  border: 0.4rem solid var(--black);
}
.input-container:focus-within {
  box-shadow: -2px 5px 8px rgba(0, 0, 0, 0.308);
}
.input-container .search {
  background-color: var(--bg-color);
  width: 90%;
  border: none;
  object-fit: fill;
  font-size: 2.2rem;
}

.main {
  background-color: var(--bg-color);
  height: auto;
  display: flex;
  justify-content: center;
}
.pokemon-list {
  margin: 10rem 0;
  border: 1px red solid;
  width: 75%;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 2rem;
}
.pokemon-container {
  color: var(--color-text);
  height: 15rem;
  background-color: var(--dark-yellow);
  border-radius: 5px;
  padding: 0 2rem;
  display: flex;
  align-items: center;
  column-gap: 2rem;
}
.poke-basic-info {
  margin: 1.5rem 0;
}
.basic-power span {
  background-color: var(--dark-yellow-opacity);
  font-size: 1.8rem;
  display: block;
  margin: 1rem 0;
}
</style>
