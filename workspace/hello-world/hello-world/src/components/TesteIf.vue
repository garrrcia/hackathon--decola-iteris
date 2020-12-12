<template>
    <div class="teste-if">
        <h1>Teste v-if</h1>
        <h2 v-if="podeVer">Agora você pode me ver</h2>
        <h2 v-else>Agora você não me ver :(</h2>
    </div>    
</template>

<script>
export default {
    name: 'TesteIf',
    data() {
        return {
            podeVer: true
        }
    }
}
</script>

<style scoped>

</style>