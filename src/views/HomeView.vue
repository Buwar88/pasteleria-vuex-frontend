<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/paslogo.png" >
    <h1>¡BENVENUTO!</h1>
    <p>Somos una pastelería tradicional italiana, conservando las formas de preparación trasnmitidas de generación en generación, con ese delicioso sabor a hogar.</p>
    <p>En nuestro menú podrás encontrar los sabores y adornos que tenemos para puedas elegir y combinar los que más te gusten.</p>
    <router-link to="/PedidoView">
    <input type="button" class="pedido" value="Realizar Pedido">
    </router-link>
  </div>
  <menuView/>
 <allFooter/>
</template>

<script>
import allFooter from "../components/footerPast.vue";
import menuView from "../components/menuView.vue";
export default{
    name:'HomeView',

    components:{
        allFooter,
        menuView,
    }

}
</script>

<style>
div{
  background-color: rgb(202, 166, 88);
}

.pedido{
  width: 200px;
  height: 50px;
  background-color: rgb(0, 0, 0);
  font-size: 20px;
  color: rgb(233, 191, 144);
  font-weight: bold;
  border-radius: 10%;
}
img{
  width : 400px; 
  height :200px;
}

</style>
