<template>
  <div class="row">
    <form>
      <div class="col-sm-8 col-sm-offset-2 col-sx-12 col-sx-offset-2 col-md-6 col-md-offset-3 form-group">
        <label for="" Quote></label>
        <textarea class="form-control" rows="3" v-model="quote"></textarea>
      </div>
      <div class="col-sm-8 col-sm-offset-2 col-sx-12 col-sx-offset-2 col-md-6 col-md-offset-3 form-group">
        <button class="btn btn-primary" @click.prevent="createNew">
          Add Quote
        </button>
      </div>
    </form>
  </div>
</template>
<script>

  export default {
    data: function() {
      return {
        quote: ''
      };
    },
    methods: {
      createNew() {
        this.$emit('quoteAdded', this.quote);
        this.quote = '';
      }
    }
  }
</script>

<style scoped>
  .btn {
    background-color: #583bb6;
    border-color: none;
    transition: 0.4s ease-out;
  }

  .btn:hover {
    background-color: #000000;
  }

</style>
