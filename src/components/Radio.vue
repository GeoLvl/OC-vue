<template>
    <div class="radio">
        <h2>Radio</h2>
        <button @click="sendMessage">Envoyer un message</button>
    </div>
</template>

<script>
export default {
    name: 'the-Radio',
    methods: {
        sendMessage() {
            this.$emit('message-sent', {
                message: 'mon magnifique message'
            })
        }
    }
}
</script>

<style scoped>
.radio {
    margin-bottom: 15px;
}
</style>