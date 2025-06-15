<script setup>
const { label, stat } = defineProps(
    {
        label: String,
        stat: String,
    }
)
</script>

<template>
    <div class="stat">
        <div class="stat__name">
            {{ label }}            
        </div>
        <div class="stat__value">
            {{ stat }}
        </div>
    </div>
</template>

<style scoped>
    .stat {
        display: flex;
        justify-content: space-between;
    }

    .stat__name {
        font-weight: 700;
        font-size: 28px;
        text-transform: uppercase;
    }

    .stat__value {
        font-weight: 500;
        font-size: 28px;
    }
</style>