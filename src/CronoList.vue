
<script>
import CronoItem from "./CronoItem.vue";
export default {
    props: ["items"],
    components: { CronoItem }
}
</script>

<template>
    <h2>Acontecimientos</h2>
    <ul>
        <CronoItem v-for="item in items" :key="item.id" :year="item.year" :text="item.text"
            :isImportant="item.isImportant" />
        <!-- <li v-for="item in items" :key="item.id">
            <span class="item-year">{{ item.year }} </span>
            <span v-html="item.text"></span>
        </li> -->
    </ul>
</template>


<style scoped>
h2 {
    color: palevioletred;
}
</style>