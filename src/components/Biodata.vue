<template>

<!-- Teknik declarative Rendering -->
    <div>
        Nama : {{ nama}} <br/>
        Umur : {{ usia }} <br />
        asal : {{asal}}
    </div>
</template>

<script>
export default {
    data(){
        return{
            nama : 'Khalid Ibrahim',
            usia : 22,
            asal: 'Kota Jambi'
        }
    },

    mounted(){
        this.usia = this.usia + 3; 
    }
}
</script>

<style scoped>

</style>