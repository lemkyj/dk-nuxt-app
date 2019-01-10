<template>
    <h1>Single user with ID: {{ $route.params.id }} </h1>
</template>

<script>
export default {
    validate (data) {
        console.log(data.params.id)
        return /^\d+$/.test(data.params.id)
    }
}
</script>
