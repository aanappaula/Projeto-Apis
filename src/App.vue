<script>
import axios from "axios";
export default {
  data() {
    return {
      cep: "",
      endereco: {},
    };
  },
  methods: {
    async buscar() {
      const url = `https://viacep.com.br/ws/${this.cep}/json/`;
      const res = await axios.get(url);
      this.endereco = res.data;
    },
  },
};
</script>

<template>
  <main>
    <h1>Buscar Cep</h1>
    <form @submit.prevent="buscar">
      <label for="rua">CEP:</label>
      <input type="text" v-model="cep" placeholder="Digite o CEP:" />
      <button type="submit">Buscar:</button>
    </form>
    <form class="end">
      <label for="rua">Rua:</label>
      <input type="text" v-model="endereco.logradouro" />
    </form>
    <form class="end">
      <label for="numero"
        >Número:
        <input type="text" v-model="endereco.numero" />
      </label>
    </form>
    <form class="end">
      <label for="Bairro">Bairro:</label>
      <input type="text" v-model="endereco.bairro" />
    </form>
    {{ endereco }}
  </main>
</template>

<style>
@import "@/assets/base.css";
@import "@/assets/main.css";
#app {
  max-width: 5000px;
  max-height: 1000px;
  margin: 0 auto;
  height: 100vh;
  font-weight: normal;
}
header,
footer {
  background-color: rgb(126, 73, 126);
  color: white;
  height: 15%;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 2rem;
}
main {
  background-color: pink;
  padding: 40px;
  border-radius: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
input {
  align-items: center;
}
</style>
