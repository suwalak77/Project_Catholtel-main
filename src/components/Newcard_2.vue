<template>
    <div class="box" style="margin: 50px;">
    <div class="col" v-for="(n) in travelList" :key="n">
      <div class="card" style="width: 50rem;" >
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
    {name:' ห้องพัก:ขนาดเล็ก/ราคา:400',   img:"https://www.thepremiercathotel.com/wp-content/uploads/2019/02/Premier-Cat-Hotel-Deluxe-room-website-homepage-2.jpg"},
    {name:' ห้องพัก:ขนาดใหญ่/ราคา:700',   img:"https://sigmafurniturestore.com/wp-content/uploads/2021/06/323658-832x1024.jpg?fbclid=IwAR1-9WRrCsF6lDu7u7ndawbW5DMVzKDA9pS9qWrsKVds69yHYV0n6aqMieA"},
    {name:' ห้องพัก:แบบรวม/ราคา:300',   img:"https://f.ptcdn.info/095/035/000/1441278336-image-o.jpg?fbclid=IwAR3f8aw5HgWhqbkqBtAnWHE-nQumDNFoKk6EHuaAhyCcp2oUDdEZ9AO8pmY"},])

</script>

<style>

.card-img-top{
height: 100%;
padding: 25px;

}
.box{
justify-content: center;
align-items: center;
margin-left: 50px;
text-align: center;

}

</style>