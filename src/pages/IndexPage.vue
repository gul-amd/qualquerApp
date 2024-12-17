<template>
  <q-page padding>
    <div class="text-center">
      <h1>Contador</h1>
      <p>Este e um contador!</p>

      <br />
      <br />
      <br />

      <!-- Botão redondo -->
      <q-btn
        icon="add"
        color="primary"
        round
        size="lg"
        @click="incrementarContador"
        class="q-mt-md"
      />
      <br />
      <br />
      <br />
      <br />
      <p class="q-mt-md">Pressione o botao acima para contar!</p>
      <p class="q-mt-md">
        <strong
          ><h2>{{ contador }}</h2></strong
        >
      </p>
      <!-- Botão de reset -->
      <q-btn
        label="Resetar Contagem"
        color="red"
        flat
        @click="resetarContador"
        class="q-mt-md q-ml-md"
      />
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      contador: 0, // Estado inicial do contador
    }
  },
  methods: {
    incrementarContador() {
      this.contador++ // Incrementa o contador a cada clique
    },
    resetarContador() {
      this.contador = 0 // Reseta o contador para zero
    },
  },
}
</script>

<style scoped>
h1 {
  color: #000;
}
</style>
