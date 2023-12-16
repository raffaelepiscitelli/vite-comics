<template>
    <img src="../assets/imgs/jumbotron.jpg" alt="">
</template>
<script>
export default {
    name: 'JumbotronHeader'

}
</script>
<style lang="scss" scoped>
@use '../styles/general.scss' as *;

img {
    height: 20.5rem;
    width: 100%;
    object-fit: cover;
    object-position: top;
    display: block;
}
</style>