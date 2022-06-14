<template>
    <div class="about container">
        <h2 class="title">What is Sneakers:</h2>
        <p class="about__subtitle">
        First ever smart contract game with passive yields in BNB directly to your own wallet. 
        All players are placed randomly in 16 levels with unlimited cycles.
        <br><br>
        Rewards are distributed as follows:
        <br>
        - 74% of level value for each of your level cycle
        <br>
        - 13%-8%-5% of level value from partners down to 3 in depth when they activate levels
        </p>
        <img src="@/assets/img/about.png" alt="" class="about__img">
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.about {
    padding-top: 12rem;
    position: relative;
}
.about__subtitle {
    font-weight: 500;
    font-size: 2rem;
    line-height: 3rem;
    max-width: 78rem;
    color: rgba(255, 255, 255, 0.5);
    padding: 1.2rem 0 50rem 0;
}
.about__img {
    position: absolute;
    top: 40rem;
    left: -4rem;

}
</style>