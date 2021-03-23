<template>
  <div>
    <div class="container-sm">
      <form>
        <div class="mb-3">
          <label for="exampleInputEmail1" class="form-label">larghezza</label>
          <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" v-model="width">
        </div>
        <div class="mb-3">
          <label for="exampleInputPassword1" class="form-label">altezza</label>
          <input type="text" class="form-control" id="exampleInputPassword1" v-model="height">
        </div>
      </form>
      <div class="btn btn-danger btn-lg" @click="cl" type="button">
        full HD (1920x1080)
      </div>
    </div>

    <img src="../assets/image.jpg" alt="taiga" :width="width" :height="height">
  </div>
</template>

<script>
export default {
  name: 'image_component',
  props: {
    height: {
      type: String,
      required: false
    },

    width: {
      type: String,
      required: false
    }
  },

  methods: {
    cl: function() {
      this.height = "1080";
      this.width = "1920";
    }
  }
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
