<script setup>

</script>

<template>
    <button class="button">
        <div>
            <slot name="icon">
            </slot>
        </div>
        <slot></slot>
    </button>
    
    
</template>

<style scoped lang="scss">
    .button {
        border: none;
        border-radius: 10px;
        background: var(--gradient);
        padding: 14px;
        font-family: var(--font);
        font-size: 20px;
        font-weight: 600;
        color: var(--primary);
        cursor: pointer;
    }

    .button:hover {
        background: var(--gradient-inverted);
    }
</style>
