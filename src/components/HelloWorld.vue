<template lang="pug">
  .container
    .d-flex.flex-column
      .h3 Choose Account Type
      // img(width="25%" src="../assets/img/logo.png")
    .d-flex.flex-row
      el-card
        svg
          img(src="../assets/img/patient.svg")
      el-card
        img(:src="img.doc") 
    .d-flex.flex-column
      el-input(value="qetuoljgd@hotamil")
      el-input(type="password" value="spdier") 
    .d-flex.flex-row
      el-button(@click="submit" type="primary") 3394
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data: () => ({
    img: {
      doc: require("../assets/img/doctor.svg")
    }
  }),
  methods: {
    submit() {
      console.log(3);
    }
  }
};
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
