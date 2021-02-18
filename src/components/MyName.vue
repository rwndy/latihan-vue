<template>
  <main>
    <h1>{{ name }}</h1>
    <h4>{{ age }}</h4>
  </main>
</template>

<script>
export default {
  name: 'MyName',
  props: {
    name: String,
    age: Number,
  },
  
}
</script>