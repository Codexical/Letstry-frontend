<template>
    <p>Current time: {{ currentTime }}</p>
</template>

<script>
export default {
    data() {
        return {
            currentTime: new Date().toLocaleTimeString()
        }
    },
    mounted() {
        setInterval(() => {
            this.currentTime = new Date().toLocaleTimeString()
        }, 1000)
    },
}
</script>
