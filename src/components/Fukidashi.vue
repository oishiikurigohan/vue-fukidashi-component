<template>
    <div class="fukidashi">
        {{ props.modelValue }}
    </div>
</template>

<script lang="ts" setup>
const props = defineProps<{
    modelValue: string
}>()
</script>

<style scoped>
.fukidashi {
    position: relative;
    display: inline-block;
    max-width: 192px;
    margin: 9px 12px;
    padding: 9px 14px;
    background: hotpink;
    color: white;
    border-radius: 19px;
    overflow-wrap: break-word;
    font-weight: bold;
}

.fukidashi::after {
    position: absolute;
    content: "";
    display: block;
    left: -10px;
    top: -21px;
    width: 24px;
    height: 36px;
    border-radius: 18px 0 6px 18px/18px 0 1px 18px;
    box-shadow: -3px -15px 0 -5px hotpink inset;
}
</style>