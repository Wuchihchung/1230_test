<template>
    <children :msg="HELLO" />
</template>

<script>
import Children from './children.vue'
import children from './components/children.vue'

export default {
    name: "num4",
    components: {
        children
    }
}
</script>