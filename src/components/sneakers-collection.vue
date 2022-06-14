<template>
    <div class="container">
        <h2 class="title">Sneakers collection</h2>
        <p class="subtitle">Special games with unique logic and mechanics fully based on smart contracts</p>
        <slot></slot>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.subtitle {
    font-weight: 500;
    font-size: 2rem;
    line-height: 3rem;
    color: rgba(255, 255, 255, 0.5);
    padding-bottom: 3rem;
    padding-top: .7rem;
}
</style>