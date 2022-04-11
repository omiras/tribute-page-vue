

<script>
export default {
    props: ["year", "text", "isImportant"],
    data() {
        return {
            importantColor: '#FFFFBF'
        }
    }
}
</script>

<template>
    <li :style="{ 'backgroundColor': isImportant ? importantColor : 'transparent' }">
        <span class="item-year">{{ year }} </span>
        <span v-html="text"></span>
    </li>
</template>

<style scoped>
.item-year {
    font-weight: bold;
}

.item-year::after {
    content: ': ';
    font-weight: bold;

}
</style>