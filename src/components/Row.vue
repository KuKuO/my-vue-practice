<template>
    <div class="row">
        <slot></slot>
    </div>
</template>
<script>
export default {
    name: 'row'
}
</script>
<style lang="scss" scoped>
.row {
    display: flex;
    > * {
        margin-bottom: 16px;
    }
    > *:not(:last-child) {
        margin-right: 24px;
    }
    flex-wrap: wrap;
}
</style>