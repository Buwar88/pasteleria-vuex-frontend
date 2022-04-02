<template>
    <div class="comanda">
        <img src="../assets/paslogo.png" alt="Logo Pastelería">
        <h1>INVENTARIO</h1>
        <saborStock/>
        <adornoStock/>
        <ordenPastel/>
    </div>

<allFooter/>
</template>

<script>
import allFooter from "../components/footerPast.vue";
import saborStock from "../components/saborStock.vue";
import adornoStock from "../components/adornoStock.vue";
import ordenPastel from "../components/ordenPastel.vue";

export default{
    name:'PasteleroView',

    components:{
        allFooter,
        saborStock,
        adornoStock,
        ordenPastel,
    }

}

</script>
<style>
img{
    width:"50px";
    height:"25px";
}
.comanda{
    align-content: center;
    align-items: center;
    display: inline-block;
    justify-content: center;
    }
</style>