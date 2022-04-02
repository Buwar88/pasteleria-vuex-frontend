<template>
    <div>
                <h3>Sabores Pastel</h3>
        <table>
            <tr>
                <th>Sabor</th>
                <th>Stock</th>
                
            </tr>
            <tr>
                <td>Chocolattiano </td>
                <td>{{ $store.state.stockChoco }}</td> 
            </tr>
            <tr>
                <td>Vanillatto </td>
                <td>{{ $store.state.stockVanillato }}</td>
            </tr>
            <tr>
                <td>Fresigglia </td>
                <td>{{ $store.state.stockFresigglia }}</td>
            </tr>
            <tr>
                <td>Tre latti </td>
                <td>{{ $store.state.stockLatti }}</td>
            </tr>
        </table>
    </div>
</template>

<script>
export default {
  name: 'saborStock',
}
</script>