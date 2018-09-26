<template>
  <div class="produto">
    <Produto titulo="Olá vamos controlar os Produtos"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Produto from '@/components/Produto.vue'

export default {
  name: 'produto',
  components: {
    Produto
  }
}
</script>
