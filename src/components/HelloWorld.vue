<template>
  <div class="hello">
    <h1>{{ msg }}</h1>

        <b-container>
      <b-jumbotron header="Bootstrap Vue"
                    lead="Bootstrap 4 Components for Vue.js 2"
      >
        <p>For more information visit our website</p>
        <b-btn variant="primary" href="https://bootstrap-vue.js.org/">More Info</b-btn>
      </b-jumbotron>

      <b-form-group horizontal
                    :label-cols="4"
                    description="Let us know your name."
                    label="Enter your name"
      >
          <b-form-input v-model.trim="name"></b-form-input>
      </b-form-group>

      <b-alert variant="success" :show="showAlert">
        Hello {{ name }}
      </b-alert>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },        
  data: {
    name: ''
  },
  computed: {
    showAlert() {
      return this.name.length > 4 ? true : false;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
