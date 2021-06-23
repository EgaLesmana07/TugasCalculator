<template>
    <h1> Loops Page</h1>
    <table border=1>
        <tr v-for="hari in namaHari" v-bind:key="hari">
            <td>{{hari}}</td>
        </tr>
    </table>
</template>

<script>
export default {
    data() {
        return{
            namaHari : ["Senin","Selasa","Rabu","Kamis","Jum'at","Sabtu","Minggu"]
        }
    }
}
</script>