<template class="row">
    <tr>
      <td>{{p.id}}</td>
      <td>{{p.name}}</td> 
    </tr>
</template>

<script>
export default {
  name: 'row-grid-produto',
  props: ['p']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
