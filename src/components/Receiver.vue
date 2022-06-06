<template>
    <div>
        <h1>Récepteur</h1>
        <radio @message-sent="updateMessage"/>
        {{ message }}
    </div>
</template>

<script>
import Radio from "./Radio.vue"

export default {
    name: 'the-Receiver',
    components: {
        Radio,
    },
    methods: {
        updateMessage(payload) {
            this.message = payload.message
        }
    },
    data: () => ({
        message: "Pas de messages"
    })
}
</script>

<style scoped lang='scss'>

</style>