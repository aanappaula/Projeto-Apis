@import "./main.css";
<template>
  <main>
    <form>
      <div class="principal mb-3">
        <label for="exampleInputEmail1" class="form-label"
          >Insira o seu CEP:</label
        >
        <input
          type="email"
          class="form-control"
          id="exampleInputEmail1"
          aria-describedby="emailHelp"
        />
        <div id="emailHelp" class="form-text">
          Seu cep não será compartilhado com ninguém!
        </div>
      </div>
      <div class="mb-3 form-check">
        <input type="checkbox" class="form-check-input" id="exampleCheck1" />
        <label class="form-check-label" for="exampleCheck1">Concordo</label>
      </div>
      <button type="submit" class="btn btn-primary">Enviar</button>
    </form>
  </main>
  <div class="principal mb-3">
    <label for="exampleInputEmail1" class="form-label">logradouro</label>
    <input
      type="email"
      class="form-control"
      id="exampleInputEmail1"
      aria-describedby="emailHelp"
    />
  </div>
  <div class="principal mb-3">
    <label for="exampleInputEmail1" class="form-label">Bairro</label>
    <input
      type="email"
      class="form-control"
      id="exampleInputEmail1"
      aria-describedby="emailHelp"
    />
  </div>
  <div class="principal mb-3">
    <label for="exampleInputEmail1" class="form-label">Cidade</label>
    <input
      type="email"
      class="form-control"
      id="exampleInputEmail1"
      aria-describedby="emailHelp"
    />
  </div>
  <div class="principal mb-3">
    <label for="exampleInputEmail1" class="form-label">uf</label>
    <input
      type="email"
      class="form-control"
      id="exampleInputEmail1"
      aria-describedby="emailHelp"
    />
  </div>
</template>
