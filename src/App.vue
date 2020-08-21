<template>
  <div id="app">
    <img
      src="https://siamrath.co.th/files/styles/1140/public/img/20191127/a90b412f49339d8eaf84096587c65daeeda24c78fbb1bc7a50039b8ba31820b9.jpg?itok=PaZcvRIG"
      class=" rounded " width="30%" height="20%"
    />
    <p><br /> </p>
    <HelloWorld msg="KAWAII !!" />
    <br />
    <div class="row">
      <div class="col-4">
        <img
          src="https://www.benarnews.org/thai/news/TH-Prawit-allegation-01162018140112.html/180116-TH-prawit-1000.jpg/@@images/cdbe68c1-c96f-4bc8-b869-f8fc24f7c3d0.jpeg"      
          class=" rounded "  width="70%" height="50%"        
        />
        <p> <br /> </p>
        <Button  />
      </div>
      <div class="col-4">
        <img
          src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQ8NcwamfTL4YYjqYj7LHa3blrr_o5JXmsZ1ReIzlEZwQ&usqp=CAU&ec=45690268"
          class="rounded "  width="70%" height="50%"        
        />
        <p>
          <br />
        </p>
        <Button />
      </div>
      <div class="col-4">
        <img
          src="https://thestandard.co/wp-content/uploads/2019/01/%E0%B8%9B%E0%B8%A3%E0%B8%B0%E0%B8%A7%E0%B8%B4%E0%B8%95%E0%B8%A3_cover-web.jpg"
          class="  rounded "  width="70%" height="50%"
        />
        <p>
          <br />
        </p>
        <Button />
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Button from "./components/Button.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Button,
  },

  data: function () {
    return {
      total: 0, //ผลรวมทั้งหมด  -->เอาไปแสดงผล {{}}
    };
  },
};
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
