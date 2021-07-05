<template>
    <div>
        <h2 class="title">La mia prima app con Vue CLI! <span @click="click">CLICCAMI!!</span></h2>
        <h3>Creato da <span class="underlin">{{ msg }}</span></h3>
    </div>
</template>

<script>
export default {
    name: 'Title',
    props: {
        msg: String
    },
    methods: {
        click: function(){
            alert('con this possiamo richiamare la proprietà --> ' + this.msg);
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .title{
        font-size: 2rem;
    }

    .underlin{
        background: yellow;
    }
</style>
