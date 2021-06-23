<template>
  <h1>Home Page</h1>
    <h4>Project Vue Pertama Saya</h4>
    <h4>Nama Saya {{ nama }} </h4>
    <h4>Umur Saya {{ tahunlahir }} tahun </h4>
    <input v-model="kotalahir"/>
    <h5> Kota Lahir Saya : {{kotalahir}} </h5>
    <button v-on:click="next">next</button>
    
</template>

<script>
export default {
  data(){
    return{
      nama : "Ega Lesmana",
      tahunlahir : 1998,
      kotalahir : "Cimahi"
    }
  },
  methods:{
    next(){
      this.tahunlahir += 1;
    }
  },
  mounted(){
    this.tahunlahir = 2021 - this.tahunlahir;
    
  }
}
</script>
