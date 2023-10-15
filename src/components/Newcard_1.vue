<template>
    <div class="box_all-mx-auto">
    <div class="col" v-for="(n,i) in travelList" :key="n">
      <div class="card" style="width: fit-content; height: fit-content;" >
        <img :src="n.img" class="card-img-top">
        <div class="card-body">
          
          <h1 class="card-title">{{ n.name }}</h1>
          <a class="btn btn-primary" @click="list_local_control(i.name, i.quantity)"> Booking </a>
          <div>
        <h4>Star cathotel<br></h4>
          <h5>Contact person : คุณดาว<br> 
              Address : xxxxxxxxxxx<br>  
              Mobile Phone : xxx-xxx-xxxx<br> 
              Line ID : @star_cathotel <br> 
              FB : Star cathotel โรงแรมแมว สตาร์แคท 
          </h5>
          </div>
          <h6>เวลาทำการ: 8.00-19.00 <br>
            <b>Location:</b> xxxxxxxxxxx</h6>      
        </div>
      </div>
    </div>
  </div>

</template>

<script setup>

import { ref } from 'vue';

const travelList=ref([
    {name: 'เกี่ยวกับเรา',   img:"https://www.petmap.co/wp-content/uploads/2020/06/106003203_1385698631627513_4277046609756839871_o.jpg", quantity: 0 , text:"TEL:087-881-7711<br>LINE:Gattocathotel" ,
        
    }])


</script>

<style>

.card-img-top{
height: 100%;
width: 100%;
padding: 40px;
border-radius: 50px;
border-top: 50px;


}
.box_all{
justify-content: center;
align-items: center;
margin-left: 100%;
text-align: center;
border-radius: 60px;


}
.btn.btn-primary{
background-color: rgb(61, 134, 216);
}

</style>