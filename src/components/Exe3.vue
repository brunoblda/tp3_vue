<template>
    <div>
        <slot>
        <p v-bind:style="{color: cor, fontSize: tamanho_texto + 'px'} ">
            {{texto}}
        </p>
        </slot>
    </div>
</template>

<script>
export default {
    name: "Exe3",
    data: function() {
        return{
            tamanho_texto: "33",
            cor: "#FF0000",
            texto: "Texto Default"

        }
    }
    
}
</script>

<style scoped>

</style>