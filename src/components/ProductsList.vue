<template>
  <div class="ProductsList">
    <ul>
        <li v-for="produto in produtos" :key="produto.id">
           {{ produto.id }}
           {{ produto.categoria }}
           {{ produto.descricao}}
           {{ produto.valor}}
        </li>
    </ul>
  </div>
</template>

<script>
export default {
   props: ["produtos", "index"]
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
