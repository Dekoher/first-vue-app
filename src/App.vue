<script>
export default {
  data: () => ({ counter: 50 }),
  methods: {
    increment() {
      this.counter++;
    },
    decrement() {
      if (this.counter > 0) {
        this.counter--;
      }
    },
    reset() {
      this.counter = 0;
    },
  },
};
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="" width="160" height="80" />
    <small>
      <h1>First Dekoher Vue App</h1>
    </small>
    <hr />
    <h2>Contador : {{ counter }}</h2>
    <button @click="increment()">+1</button>
    <button @click="decrement()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
}

small {
  color: #666;
}

h1 {
  font-weight: 700;
}

h2 {
  font-size: 2.5rem;
}

button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0 8px;
  padding: 0.5rem;
}
</style>
