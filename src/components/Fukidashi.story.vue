<script lang="ts" setup>
import { ref } from 'vue'
import Fukidashi from "./Fukidashi.vue"
const text = ref('histoire dev')
</script>

<template>
    <Story title="withProps">
        <Fukidashi v-model="text" />
    </Story>
</template>