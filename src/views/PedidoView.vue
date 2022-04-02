<template>
    <div class="secPed">
        <img src="../assets/paslogo.png" alt="Logo Pastelería">
        <formularioView/>
    </div>
  <allFooter/>  
</template>

<script>
import allFooter from "../components/footerPast.vue";
import formularioView from "../components/formularioView.vue";
export default {
name:'PedidoView',

components:{
    allFooter,
    formularioView,
},
};

</script>
 

<style>

.secPed {
    background-color: rgb(202, 166, 88);
    font-family: Arial, Helvetica, sans-serif;
}
img{
    width:"50px";
    height:"25px";
}

footer {
   background-color: rgb(7, 7, 7);
   padding: 10px;
   text-align: center;
   color: white;
}
</style>