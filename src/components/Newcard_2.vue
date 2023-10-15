<template>
    <div class="box_all">
    <div class="col" v-for="(n) in travelList" :key="n">
      <div class="card" style="width: 60rem;" >
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
    {name:' ห้องพัก:ขนาดเล็ก/ราคา:400',   img:"https://www.chillpainai.com/src/wewakeup/scoop/img_scoop/scoop/jajah_student/cat%20hotel/cat6_1.jpg"},
    {name:' ห้องพัก:ขนาดใหญ่/ราคา:700',   img:"https://www.chillpainai.com/src/wewakeup/scoop/img_scoop/scoop/jajah_student/cat%20hotel/cat8_1.jpg"},
    {name:' ห้องพัก:แบบรวม/ราคา:300',   img:"https://www.chillpainai.com/src/wewakeup/scoop/img_scoop/scoop/jajah_student/cat%20hotel/cat1_1.jpg"},])

</script>

<style>

.card-img-top{
height: 100%;
padding: 25px;

}
.box_all{
justify-content: center;
align-items: center;
margin-left: 50px;
margin-right: 50px;
text-align: center;
border-radius: 60px;

}

.card{
justify-content: center;
margin: 100px;
margin-top: 50px;
text-align: center;
}

</style>