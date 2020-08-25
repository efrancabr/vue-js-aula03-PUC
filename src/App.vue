<template>
  <div id="app">

    <span> OLA </span>

    <ProductsList produtos="produtos">

  

  </div>
</template>

<script>
import ProductsList from './components/ProductsList';

export default {
  name: 'App',
  components: {
    ProductsList
  },
 data() {
   return { 
   produtos: [  
        {
            id: '1',
            categoria: 'Celulares',
            descricao: 'Iphone 11 dourado',
            publishedAt: '2020-08-25'
        },
        {
            id: '2',
            categoria: 'Notebooks',
            descricao: 'Notebook Dell Ispiron',
            publishedAt: '2020-08-15'
        },
        {
            id: '3',
            categoria: 'Eletronicos',
            descricao: 'Cafeteira',
            publishedAt: '2020-08-25'
        }
    ]
  }
 }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
