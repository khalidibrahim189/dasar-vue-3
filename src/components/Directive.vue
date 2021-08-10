<template>
    <div>
        <h2>Belajar Directive</h2>

        <div>
            <p>Data bilangan ganjil</p>
            <h2>Angka : {{ bilangan }}</h2>
            <button v-on:click="next">Tekan</button>
        </div>
    </div>
</template>


<script>
export default {
    data(){
        return{
            bilangan : 1,
        }
    },

    methods:{
        next(){
            this.bilangan += 2;
        }
    }
}
</script>