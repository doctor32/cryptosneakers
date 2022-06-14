<template>
    <div class="collection__body">
        <h4 class="collection__body_title">{{title}}</h4>
        <div class="collection__body_items">
            <slot></slot>
        </div>
        <a href="">
            <button class="btn">{{buttonText}}</button>
        </a>
    </div>
</template>

<script>
    export default {
        props: ['title', 'buttonText']
    }
</script>

<style lang="scss" scoped>
.collection__body {
    background: rgba(255, 255, 255, 0.03);
    backdrop-filter: blur(20rem);
    /* Note: backdrop-filter has minimal browser support */
    border-radius: 1.5rem;
    padding: 3.6rem 4.8rem 5.6rem 4.8rem;
    display: flex;
    flex-direction: column;
    
}
.collection__body_title {
    align-self: flex-start;
    font-weight: 700;
    font-size: 3.6rem;
    line-height: 4.4rem;
    /* identical to box height */
    color: #FFFFFF;
    padding-bottom: 3.6rem;
}
.collection__body_items {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    row-gap: 3rem;
}
a {
    margin: 0 auto;
}
.btn {
    background: #EA9A23;
    border-radius: 5rem;
    padding: 1.3rem 2.1rem;
    font-weight: 600;
    font-size: 1.8rem;
    line-height: 2.1rem;
    text-align: center;
    color: #FFFFFF;
    margin-top: 5.7rem;
    transition: .3s;
    &:hover{
        background: #dda24a;
    }

}
</style>