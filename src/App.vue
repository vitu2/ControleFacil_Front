<template>
  <div id="app">
    <header>
      <h1>CF - Controle Fácil</h1>
      <a href="">Inicio</a>
      <a href="">Funcionalidades</a>
      <a href="">Preços</a>
      <button @click="requestDemo">Solicitar Demonstração ✨</button>
    </header>

    <section class="features">
      <h2>Funcionalidades</h2>
      <ul>
        <li>Gestão de Estoque</li>
        <li>Controle Financeiro</li>
        <li>Vendas e Compras</li>
        <li>Relatórios Avançados</li>
      </ul>
    </section>

    <section class="benefits">
      <h2>Benefícios</h2>
      <p>Aumente a produtividade e tome decisões mais informadas.</p>
      <p>Transforme seu processo de gestão com uma interface intuitiva.</p>
    </section>

    <footer>
      <p>Entre em contato conosco: contato@erp.com</p>
    </footer>
  </div>
</template>

<script>
export default {
  methods: {
    requestDemo() {
      alert('Solicitação de demonstração enviada!');
    },
  },
};
</script>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  text-align: center;
}

div header {
  background-color: #10403B;
  color: #f0f0f0;
  display: flex;
  justify-content: space-around;
  align-items: center;
  border-radius: 20px;
  padding: 10px;
}

header button {
  height: 3rem;
  padding: 10px 20px;
  border-radius: 12px; 
  border: none;
  cursor: pointer;
  background-color: #0c2b26; 
  color: rgb(130, 212, 22);
  font-size: 1.1em; 
  font-weight: bold; 
  transition: background-color 0.3s, transform 0.3s ease;
}

header button:hover {
  background-color: rgb(128, 156, 24);
  color: rgb(26, 41, 7);
}

div header a{
  background-color: #127369;
  color:#f0f0f0 ;
  padding: 6px;
  border-radius: 8px;
  text-decoration: none;
}

div header a:hover{
  background-color: #326927;
  padding: 6px;
  border-radius: 8px;
  text-decoration: none;
  transition: .4s;
}

header h1 {
  font-size: 3em;
}

.features,
.benefits {
  margin-top: 40px;
}

ul {
  list-style-type: none;
}

footer {
  margin-top: 50px;
  background-color: #f1f1f1;
  padding: 10px;
}
</style>
