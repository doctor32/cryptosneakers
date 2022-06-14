<template>
    <div class="item">
        <img class="item__bg-blur" src="@/assets/img/sneaker-bg-bw.png" alt="">
        <img class="item__sneaker" src="@/assets/img/sneaker-bw.png" alt="">
        <div class="item__bottom">
            <p class="item__title">Open your Sneaker</p>
            <button class="item__btn">
                Activate 4
                <img src="@/assets/img/lightning.png" alt="" />
            </button>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.item {
    width: 46.9rem;
    height: 38rem;
    background: rgba(54, 54, 55, 0.56);
    border: .1rem solid #979797;
    border-radius: 1rem;
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.item__bg-blur {
    position: absolute;
    top: -2rem;
    width: 30rem;
}
.item__sneaker {
    width: 17rem;
    position: absolute;
    top: 3.5rem;
}
.item__bottom {
    margin-top: 26.5rem;
    width: 100%;
    border-top: .1rem solid #979797;
    display: flex;
    align-items: center;
    flex-direction: column;
}
.item__title {
    padding: 1.6rem 0 1.8rem 0 ;
    font-weight: 700;
    font-size: 1.8rem;
    line-height: 2rem;
}
.item__btn {
    font-weight: 600;
    color: white;
    font-size: 1.6rem;
    line-height: 2rem;
    border: .2rem solid #EA9A23;
    width: 17rem;
    height: 4rem;
    display: flex;
    justify-content: center;
    align-items: center;
    filter: drop-shadow(0 0 2.5rem rgba(235, 131, 56, 0.4));
    border-radius: 3rem;
    background: rgba(255, 0, 0, 0);
    img {
        width: 1.6rem;
        padding-left: .5rem;
    }
    background-image: linear-gradient(#EA9A23, #EA9A23);
    background-position: 50% 50%;
    background-repeat: no-repeat;
    background-size: 0% 100%;
    transition: background-size .5s, color .5s;
    &:hover {
    background-size: 100% 100%;
}
}
</style>