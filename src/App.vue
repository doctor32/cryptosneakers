<template>
  <div>
    <img src="@/assets/img/blur-bg.png" alt="" class="bg__pic" />
    <div class="body">
      <div class="body__left">
        <vNavbar />
      </div>
      <div class="body__right">
        <header>
          <div class="container header__container">
            <div class="balance">
              Balance: <span>65</span>
              <img src="@/assets/img/lightning.png" alt="" />
            </div>
            <div class="header__right">
              <a class="connect__wallet">
                <svg
                  width="13"
                  height="12"
                  viewBox="0 0 13 12"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M6.39737 0V12M0 6.09474H13"
                    stroke="#D7BF9B"
                    stroke-width="1.3"
                  />
                </svg>
                Connect Wallet
              </a>
              <div class="header__avatar">
                <img src="@/assets/img/avatar.png" alt="header__avatar_img" />
              </div>
            </div>
          </div>
        </header>
        <main>
          <userInfo />
          <sneakers-collection>
            <collection-body
              title="My collection"
              buttonText="To programm view"
            >
              <notOpenedItem />
              <notOpenedItem />
              <notOpenedItem />
              <notOpenedItem />
            </collection-body>
          </sneakers-collection>
          <myTeam />
          <vAbout />
        </main>
        <footer>
          <div class="container footer">
            <p class="copyright">© 2022 Sneaker. All Rights Reserved</p>
            <a class="footer_link">Disclaimer</a>
          </div>
        </footer>
      </div>
    </div>
  </div>
</template>

<script>
import userInfo from "@/components/user-info.vue";
import vNavbar from "@/components/v-navbar.vue";
import sneakersCollection from "@/components/sneakers-collection.vue";
import collectionBody from "@/components/collection-body.vue";
import notOpenedItem from "@/components/not-opened-item.vue";
import myTeam from "@/components/my-team.vue";
import vAbout from "@/components/v-about.vue";
// import vHeader from "@/components/v-header";

export default {
  components: { userInfo, vNavbar, sneakersCollection, collectionBody, notOpenedItem, myTeam, vAbout },
};
</script>

<style lang="scss" scoped>
.body {
  margin: 4.5rem 8rem 6.5rem 8rem;
  background: rgba(30, 31, 32, 0.17);
  border: 0.15rem solid rgba(255, 255, 255, 0.14);
  backdrop-filter: blur(0.4rem);
  /* Note: backdrop-filter has minimal browser support */
  border-radius: 6rem;
  width: 176rem;
  min-height: 107rem;
  display: flex;
}
.bg__pic {
  position: absolute;
  width: 57rem;
  height: 82rem;
  top: 0;
  left: 30rem;
}
.body__right {
  width: 130rem;
  display: flex;
  flex-direction: column;
}
.header__container {
  display: flex;
  justify-content: space-between;
}
header {
  display: flex;
  padding: 3.1rem 0;
  border-bottom: 0.1rem solid rgba(255, 255, 255, 0.15);
  .balance {
    padding: 1rem 3.2rem;
    background: rgba(54, 54, 55, 0.56);
    border: 0.1rem solid #979797;
    border-radius: 1rem;
    display: flex;
    font-size: 3rem;
    font-weight: 300;
    align-items: center;
    span {
      font-weight: 600;
      padding-left: 0.7rem;
    }
    img {
      width: 2.2rem;
      height: 1.9rem;
      padding-left: 0.7rem;
    }
  }
  .header__right {
    display: flex;
    gap: 2rem;
    align-items: center;
  }
  .header__avatar {
    border-radius: 50%;
    width: 4rem;
    height: 4rem;
    img {
      border-radius: 50%;
    }
  }
  .connect__wallet {
    background: rgba(255, 255, 255, 0.05);
    border: 0.1rem solid rgba(215, 191, 155, 0.33);
    border-radius: 10rem;
    font-weight: 600;
    font-size: 1.6rem;
    line-height: 1.9rem;
    display: flex;
    gap: 0.6rem;
    align-items: center;
    padding: 1.2rem 2.3rem;
    svg {
      width: 1.2rem;
      height: 1.2rem;
    }
  }
}
footer {
  padding-bottom: 5.2rem;
  margin-top: auto;
  padding-top: 9rem;
  font-size: 1.6rem;
  .copyright {
    color: #929293;
  }
  .footer {
    display: flex;
    justify-content: space-between;
  }
}
.body__left {
  width: 47rem;
  border-right: 0.1rem solid rgba(255, 255, 255, 0.15);
}
</style>
