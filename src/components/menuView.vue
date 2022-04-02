<template>
  <section>
    <div>
      <h4>PASTELES</h4>
      <table>
          <tr>
              <th>Sabor</th>
              <th>Descripción</th>
              <th>Precio</th>
          </tr>
          <tr>
              <td>Chocolattiano </td>
              <td>Clásico de chocolate semi-amargo</td>
              <td>{{ $store.state.pChocolattiano }}</td>
          </tr>
          <tr>
              <td>Vanillatto </td>
              <td>Hecho con vainas directamente traídas desde Italia</td>
              <td>{{ $store.state.pVanillato }}</td>
          </tr>
          <tr>
              <td>Fresigglia </td>
              <td>Preparado con fresas orgánicas frescas</td>
              <td>{{ $store.state.pFresigglia }}</td>
          </tr>
          <tr>
              <td>Tre latti </td>
              <td>El clásico de 3 leches de la mas alta calidad</td>
              <td>{{ $store.state.pLatti }}</td>
          </tr>
      </table>
    </div>
    <div>
      <h4>ADORNOS</h4>
      <table>
        <tr>
          <th>Tipo</th> 
          <th>Descripción</th>
          <th>Precio</th> 
        </tr>
        <tr>
          <td>Letrero Chocolate</td>
          <td>Letrero hecho en chocolate semi-amargo</td>
          <td>{{ $store.state.aLetrero }}</td>
        </tr>
        <tr>
          <td>Corona Chantilly</td>
          <td>Corona en el pastel hecha de Chantilly con crema de alta calidad y un toque de vainilla</td>
          <td>{{ $store.state.aChantilly }}</td>
        </tr>
        <tr>
          <td>Fondant</td>
          <td>Cubierta fondant blanca para todo el pastel</td>
          <td>{{ $store.state.aFondant }}</td>
        </tr>
        <tr>
          <td>Rosas</td>
          <td>6 Rosas rojas y rosas comestibles</td>
          <td>{{ $store.state.aRosas }}</td>
        </tr>
      </table>
    </div>
  </section>
</template>
<script>


export default {
  name: 'menuView',
}

</script>

<style>
section{
  display: inline-flex;
  flex-wrap: nowrap;
}
  section div{
    border-style: groove;
    border-color: black;
    padding: 10px;
    border-radius: 10%;
  }
</style>