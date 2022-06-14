<template>
    <div class="team container">
        <h2 class="title">My team</h2>
        <div class="team__body">
            <div class="team__score">
                <div class="team__score_titles">
                    <p class="team__score_title">Line</p>
                    <p class="team__score_title">Collectors</p>
                    <p class="team__score_title">Sneakers Quantity</p>
                    <p class="team__score_title">Total cash</p>
                </div>
                <div class="team__score_hr"></div>
                <div class="team__score_stats">
                    <p class="team__score_stats_num">1</p>
                    <p class="team__score_stats_num">10</p>
                    <p class="team__score_stats_num">48</p>
                    <p class="team__score_stats_num">1500 ⚡️</p>
                </div>
                <div class="team__score_stats">
                    <p class="team__score_stats_num">2</p>
                    <p class="team__score_stats_num">1124</p>
                    <p class="team__score_stats_num">4800</p>
                    <p class="team__score_stats_num">30 ⚡️</p>
                </div>
                <div class="team__score_stats">
                    <p class="team__score_stats_num">3</p>
                    <p class="team__score_stats_num">20</p>
                    <p class="team__score_stats_num">99</p>
                    <p class="team__score_stats_num">1250 ⚡️</p>
                </div>
                    <div class="team__score_stats">
                    <p class="team__score_stats_num">4</p>
                    <p class="team__score_stats_num">100</p>
                    <p class="team__score_stats_num">480000</p>
                    <p class="team__score_stats_num">1500 ⚡️</p>
                </div>
            </div>
            <div class="personal__link">
                <div class="personal__link_top">
                    <div class="personal__link_top-right">
                        <p class="personal__link_title">My personal link</p>
                        <p class="personal__link_name">sneakers/8zkdki</p>        
                    </div>
                    <img class="personal__link-logo" src="@/assets/img/logo.png" alt="">
                </div>
                <div class="personal__link_bottom">
                    <button class="personal__link_btn btn__orange">Copy</button>
                    <button class="personal__link_btn btn__purple">Share</button>
                    <img src="@/assets/img/personal-link.png" alt="img" class="personal__link_bottom-img">
                </div>
                <div class="personal__link_hr"></div>
                <p class="personal__link_profit">
                Total profit team: <span>15000</span>
                <img src="@/assets/img/lightning.png" alt="" />
                </p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.team {
    padding-top: 10rem;
}
.team__body {
    display: flex;
    gap: 2.7rem;
    margin-top: 3rem;
}
.title {
}
.team__score {
    background: #1C1C1D;
    backdrop-filter: blur(20rem);
    /* Note: backdrop-filter has minimal browser support */
    border-radius: 1.5rem;
    padding: 3rem 4rem;
    width: 64.5rem;
}
.team__score_titles {
    display: flex;
    justify-content: space-between;
}
.team__score_title {
    font-weight: 500;
    font-size: 1.4rem;
    line-height: 1.5rem;
    color: #6B6B6B;
    max-width: 10rem;
}
.team__score_hr {
    margin: 1.2rem 0 3rem 0;
    background: rgba(255, 255, 255, 0.26);
    width: 100%;
    height: .1rem;
}
.team__score_stats {
    display: flex;
}
.team__score_stats_num {
    padding-bottom: 1.8rem;
    width: 13rem;
    font-weight: 500;
    font-size: 1.5rem;
    line-height: 1.6rem;
    &:nth-child(2) {
        width: 16.8rem;
    }
    &:last-child {
        padding-left: 7.4rem;
    }
}
.personal__link {
    background: rgba(34, 74, 111, 0.26);
    box-shadow: 0 .4rem 6rem rgba(74, 190, 227, 0.33), inset 0px 0px 8rem rgba(59, 148, 199, 0.41);
    backdrop-filter: blur(5rem);
    border-radius: 1.5rem;
    width: 100%;
    padding: 2.5rem 2rem 0 2rem;
    height: 24rem;
}
.personal__link_top {
    display: flex;
    justify-content: space-between;
    margin-bottom: 2.2rem;
}
.personal__link_top-right {
}
.personal__link_title {
    padding-bottom: 1rem;
    font-weight: 500;
    font-size: 1.4rem;
    line-height: 1.8rem;
    /* identical to box height, or 129% */
}
.personal__link_name {
    font-weight: 700;
    font-size: 3rem;
    line-height: 1.8rem;
}
.personal__link-logo {
    width: 5.8rem;
}
.personal__link_bottom {
    display: flex;
}
.personal__link_btn {
    border: .1rem solid #FFC700;
    border-radius: 5rem;
    background: rgba(255, 0, 0, 0);
    color: #FF9F10;
    padding: 1rem 2.2rem;
    font-weight: 500;
    font-size: 1.8rem;
}
.btn__orange {
}
.btn__purple {
    background: rgba(185, 57, 204, 0.1);
    border-color: #AB2CBF;
    color: #F29AFF;
    margin-left: 1rem;
}
.personal__link_bottom-img {
    width: 4.7rem;
    margin-left: auto;
}
.personal__link_hr {
    margin: 2.6rem 0 2.1rem 0;
    width: 100%;
    background: #4AC7E3;
    height: .1rem;
}
.personal__link_profit {
    display: flex;
    gap: 1rem;
    font-weight: 300;
    font-size: 2.4rem;
    line-height: 2.8rem;
    span {
        font-weight: 600;
    }
    img {
        width: 2.5rem;
    }
}
</style>