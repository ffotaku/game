<template>
  <div>
    <button @click="upFunction" class="btn btn-info">{{lable}}</button>
    <button @click="downFunction" class="btn btn-info ml-3">{{lable}}</button>
    <p v-bind:style="{ fontSize: fsize + 'px' }">{{ counter }}</p>
   
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      counter: 0,
      fsize: 50,
    };
  },

  props: {
    lable: String,
  },

  methods: {
    upFunction: function () {
      this.counter += 1;
      this.fsize += 10;

      //console.log('fsize =' +this.fsize);
      //console.log('counter =' +this.counter);

      //ส่งค่าตัวแปร counter ออกไปโดยผ่านตัวแปร cc
      this.$emit('cc',this.counter)

    },

    downFunction: function () {
      this.counter -= 1;
      this.fsize -= 10;

      console.log(this.fsize);
      console.log(this.counter);
    },
  },
};
</script>


<style>
</style>

