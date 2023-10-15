<template>
    <div class="box_all" style="margin: 50px;">
    <div class="col" v-for="(n,i) in travelList" :key="n">
      <div class="card" style="width: 25rem;" >
        <img :src="n.img" class="card-img-top">
        <div class="card-body">
          <h3 class="card-title">{{ n.name }}</h3>
          

        </div>
      </div>
    </div>

    <div class="col" v-for="(n,i) in travelList" :key="n">
      <div class="card" style="width: 25rem;" >
        <img :src="n.img" class="card-img-top">
        <div class="card-body" st>
          <h3 class="card-title">{{ n.name }}</h3>
          

        </div>
      </div>
    </div>
    <div class="col" v-for="(n,i) in travelList" :key="n">
      <div class="card" style="width: 25rem; " >
        <img :src="n.img" class="card-img-top">
        <div class="card-body">
          <h3 class="card-title">{{ n.name }}</h3>
          

        </div>
      </div>
    </div>
  </div>

</template>

<script setup>

import { ref } from 'vue';

const travelList=ref([
    {name:' ห้องพักและราคา',   img:"https://chiangmaicheckin.com/pic/cover/s5.jpg", img:"https://chiangmaicheckin.com/pic/cover/s5.jpg", quantity: 0 ,
    }])

</script>

<style>

.card-img-top{
height: 100%;
padding: 25px;

}
.box_all{
justify-content: center;
align-items: center;
margin-left: 30%;
text-align: center

}

</style>