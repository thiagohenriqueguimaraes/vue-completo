<template>
  <div class="produto">
    <h1>Lista de produtos</h1>
    <div class="row">
      <div class="col-md-12">
        <table style="width:100%">
              <tr>
                <th>Códito</th>
                <th>Nome</th> 
              </tr>
              <tbody>
                <gridProduto
                  v-for="p in [{ id: 1, name: 'A' },{ id: 2, name: 'B' }, { id: 3, name: 'C' }]"
                  v-bind:key="p.id"
                  v-bind:p="p"
                ></gridProduto>
              </tbody> 

            </table>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <table style="width:100%">
              <tr>
                <th>Código</th>
                <th>Nome</th> 
              </tr>
              <tbody>
                <tr v-for="x in xs">
                  <td>{{x.y}}</td>
                  <td></td>                  
                </tr>
              </tbody> 

            </table>
      </div>
    </div>
    
  </div>
</template>

<script>
// @ is an alias to /src
import gridProduto from '@/components/gridProduto.vue'

export default {
  name: 'produto',
  data () {
    return {
      xs : [{y:1}]
    }
  },
  components: {
    gridProduto
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>