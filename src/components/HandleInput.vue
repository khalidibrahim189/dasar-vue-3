<template>
    <div>
        <h2>Handle user input 2 | Handle Input</h2>
        <p> v-model : dapat digunakan sebagai two way data binding </p>
        <h5>Nama :  {{ nama }} </h5>
        <input v-model="nama" />  

    </div>
</template>

<script>
export default {
    data(){
        return{
            nama : '',

        }
    },
}
</script>