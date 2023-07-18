<template>
    <div>
        "okokoko"
    </div>
</template>

<script>
import { onMounted } from 'vue';

export default {
    name: "Person",
    props: {
        name: {
            type: String,
            required: true
        },
        salary: {
            type: Number,
            default: 15000
        }
    },
    onMounted() {
        console.log(index)
    }
}

</script>

<style scoped>
div {
    color: white
}
</style>
