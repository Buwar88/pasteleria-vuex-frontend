<template>
    <div class="contact">
        <h1 class="title">Pedido</h1>
        <form action class="form" @submit.prevent="pedido">
        <label class="form-label" for="#name">Nombre</label>
        <input
            v-model="name"
            class="form-input"
            type="text"
            id="name"
            required
            placeholder="Nombre"
        >
        <label class="form-label" for="#email">Email</label>
        <input
            v-model="email"
            class="form-input"
            type="email"
            id="email"
            placeholder="Email"
        >
        <label class="form-label" for="#telefono">Teléfono</label>
        <input
            v-model="phone"
            class="form-input"
            type="phone"
            id="phone"
            placeholder="Telefono"
        >
          <h2>Selecciona el sabor</h2>
          <label class="form-label" for="#sabor1">Chocolattiano</label>
          <input
            v-model="sabor1"
            class="form-input"
            type="checkbox"
            id="sabor1"
            placeholder="Chocolattiano"
          >
          <label class="form-label" for="#sabor2">Vanillatto</label>
          <input
            v-model="sabor2"
            class="form-input"
            type="checkbox"
            id="sabor2"
            placeholder="Vanillatto"
          >
          <label class="form-label" for="#sabor3">Fresigglia</label>
          <input
            v-model="sabor3"
            class="form-input"
            type="checkbox"
            id="sabor3"
            placeholder="Fresigglia"
          >
          <label class="form-label" for="#sabor4">Tre latti</label>
          <input
            v-model="sabor4"
            class="form-input"
            type="checkbox"
            id="sabor4"
            placeholder="Tre latti"
          >
          <h2>Selecciona tus Adornos</h2>
          <label class="form-label" for="#ad1">Letrero Chocolate</label>
          <input
            v-model="ad1"
            class="form-input"
            type="checkbox"
            id="ad1"
            placeholder="Letrero"
          >
          <label class="form-label" for="#ad2">Corona Chantilly</label>
          <input
            v-model="ad2"
            class="form-input"
            type="checkbox"
            id="ad2"
            placeholder="Corona"
          >
          <label class="form-label" for="#ad3">Fondant</label>
          <input
            v-model="ad3"
            class="form-input"
            type="checkbox"
            id="ad3"
            placeholder="Fondant"
          >
          <label class="form-label" for="#ad4">Rosas</label>
          <input
            v-model="ad4"
            class="form-input"
            type="checkbox"
            id="ad4"
            placeholder="Rosas"
          >
        <input class="form-submit" type="submit" value="Enviar">
        </form>
        </div>
</template>

<script>
export default {
  name: 'formularioView',

data: () => ({
    name: "",
    email: "",
    phone:"",
    sabor1:"",
    sabor2:"",
    sabor3:"",
    sabor4:"",
    ad1: "",
    ad2: "",
    ad3: "",
    ad4: "",
  }),

  methods: {
    
    pedido(){
      console.group("Datos");
        console.log(this.name);
        console.log(this.email);
        console.log(this.phone);
      console.groupEnd();
      console.group("Sabores");
        console.log("Chocolattiano",this.sabor1);
        console.log("Vanillatto",this.sabor2);
        console.log("Fresigglia",this.sabor3);
        console.log("Tre latti",this.sabor4);
      console.groupEnd();
      console.group("Adornos");
        console.log("Letrero Chocolate",this.ad1);
        console.log("Corona Chantilly",this.ad2);
        console.log("Fondant",this.ad3);
        console.log("Rosas",this.ad4);
      console.groupEnd();
    }
  }
}
</script>