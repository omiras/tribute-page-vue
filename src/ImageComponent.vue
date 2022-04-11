
<script>
export default {
    props: ["image", "legend"]
}
</script>

<template>
    <figure id="img-div">
        <img id="image" :src="image" :alt="legend">
        <figcaption id="img-caption"> {{ legend }} </figcaption>
    </figure>
</template>


<style>
</style>