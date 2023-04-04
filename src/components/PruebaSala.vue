
<template>
        <table  class="table table-striped table-hover">
            <thead>
                <tr>
                <th scope="col"></th>
                <th scope="col">Nombre</th>
                <th scope="col">Apellido</th>
                <th scope="col">Fecha de Nacimiento</th>
                <th scope="col">Edad</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(item,index) in usuario" :key="item.edad">
                    <th scope="row">{{index+1}}</th>
                    <td>{{item.nombre}}</td>
                    <td>{{item.apellido}}</td>
                    <td>{{item.fecha_nac}}</td>
                    <td>{{item.edad}}</td>
                </tr>
            </tbody>
        </table>



    <!-- <h2> hola prueba 2</h2>
    <ul>
        <li v-for="item in usuario" :key="item.edad">
            {{ item.nombre }} - {{ item.apellido }} - {{ item.fecha_nac }} - {{ item.edad }} -->
            <!-- {{ MensajePadre }} - {{ index }} - {{ item.nombre }} - {{ item.apellido }} - {{ item.fecha_nac }} - {{ item.edad }} -->

        <!-- </li>
 
    </ul> -->
</template>
<script>

export default {
        name: 'PruebaSala',
        data: function() {
            return {
                MensajePadre:"Usuario",
                usuario:[{ 
                   nombre: "Myrian",
                    apellido: "Barrera Cornejo",
                    fecha_nac: "06/05/1972",
                    edad: 50
                },
                { 
                   nombre: "Armando",
                    apellido: "Barrera Cornejo",
                    fecha_nac: "02/04/1976",
                    edad: 47
                },
                { 
                   nombre: "Eduardo",
                    apellido: "Barrera Cornejo",
                    fecha_nac: "18/12/1974",
                    edad: 49
                }               
            ]
            }
            
        }
    };
</script>

<style >
</style>