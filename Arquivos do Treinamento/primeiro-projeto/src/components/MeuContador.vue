<template>
    <div class="meu-contador">
        <h2>Meu contador</h2>
        <p><strong>Contador:</strong> {{ contador }}</p>
        <button @click="removerUm">-</button>
        <button @click="somarUm">+</button>
    </div>
</template>

<script>
export default {
    name: 'MeuContador',
    data() {
        return {
            contador: 0
        }
    },
    methods: {
        somarUm() {
            this.contador++;
        },
        removerUm() {
            this.contador--;
        }
    }
}
</script>

<style scoped>

</style>
