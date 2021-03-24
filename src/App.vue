<template>
  <div class="banner">
    <div id="nav">
      <div class="inner-wrapper">
        <a href="app.vue"
          ><img class="logo" src="@/assets/logo-header-white.png" alt="logo"
        /></a>

        <div class="menu">
          <ul class="nav-links">
            <li><a href="#section-cm">Community Management </a></li>
            <li><a href="#section-factures">Factures</a></li>
            <li><a href="#section-tarifs">Tarifs</a></li>
          </ul>
          <hr class="separate-line-1" />
        </div>
      </div>
    </div>

    <h1>Placez vos réseaux sociaux en pilote automatique</h1>
    <h3>Votre community manager dédié pour un prix imbattable</h3>
    <p class="animate__animated animate__fadeInUp animate__infinite">
      Swipe up
      <i class="fas fa-chevron-up"></i>
    </p>
  </div>

  <div class="section-logos">
    <Logos />
  </div>
  <div class="communitymanagement" id="section-cm">
    <CM />
  </div>

  <div class="factures" id="section-factures">
    <Factures />
  </div>

  <div class="tarifs" id="section-tarifs">
    <Pricing />
  </div>

  <div class="footer">
    <div class="frame">
      <div class="upper-frame">
        <div class="box-1">
          <img src="@/assets/logo-header-white.png" class="logo-footer" />
          <div class="social-links">
            <li class="logo-fb">
              <a href="#"><i class="fab fa-facebook-square"></i></a>
            </li>
            <li>
              <a href="#"><i class="fab fa-twitter"></i></a>
            </li>
            <li>
              <a href="#"><i class="fab fa-instagram"></i></a>
            </li>
          </div>
        </div>
        <div class="box-3">
          <a href="#" class="title-footer-section"> À propos de Koliagram </a>
          <ul>
            <li><a href="#section-cm"> Community Management </a></li>
            <li><a href="#section-factures"> Factures </a></li>
            <li><a href="#section-tarifs"> Tarifs </a></li>
            <li>
              <a href="#">
                Envie d'en savoir plus ? Contactez-nous au 06.58.68.21.51
              </a>
            </li>
          </ul>
        </div>
      </div>
      <hr class="separate-line" />
      <div class="bottom-line">
        <h3>Made with ❤️ in Paris</h3>
      </div>
    </div>
  </div>
</template>

<script>
import Pricing from "@/components/Pricing.vue";
import CM from "@/components/CommunityM.vue";
import Factures from "@/components/Factures.vue";
import Logos from "@/components/Logos.vue";

export default {
  name: "App",
  components: {
    Pricing,
    CM,
    Factures,
    Logos,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");

body {
  margin: 0px;
}

#app {
  font-family: "Roboto", sans-serif;
}

#nav {
  //position: fixed;
  z-index: 5;
  top: 0;
  left: 0;
  width: 100%;
  transition: background 0.35s;

  .inner-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 200px;
    height: 70px;
  }

  a {
    font-weight: bold;
    color: white;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.logo {
  cursor: pointer;
  width: 150.5px;
  height: 99.5px;
}

.nav-links li {
  display: inline-block;
  padding: 0px 20px;
}

.nav-links li a {
  font-family: "Roboto", sans-serif;
  font-size: 16px;
  text-decoration: none;
  list-style: none;
  transition: all 0.3s ease 0s;
}

.nav-links li a:hover {
  color: grey;
  text-decoration: none;
}

.separate-line-1 {
  margin: 3px 62px;
  margin-right: 35px;
  margin-left: 80px;
}

.banner {
  width: 100%;
  height: 100vh;
  //padding: 0px 20px 345px 40px;
  background-size: cover;
  background-position: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.9), rgba(0, 0, 0, 0.4)),
    url("./assets/background-marine.jpg");

  h1 {
    color: white;
    font-size: 50px;
    text-align: center;
    margin-top: 15rem;
  }
  h3 {
    color: white;
    font-size: 20px;
    font-weight: lighter;
    text-align: center;
    margin-top: 2rem;
  }
  p {
    color: white;
    text-align: center;
    font-size: 21px;
    margin-top: 10rem;
  }
  .animate__fadeInUp {
    --animate-duration: 2s;
  }
}

.communitymanagement {
  background-color: #f7f9fc;
}
.communitymanagement,
.factures {
  padding: 2rem;
}
.tarifs {
  padding-top: 2rem;
  padding-left: 2rem;
  padding-right: 2rem;
}

.footer {
  padding: 72px 0px 88px;
  background-color: #000000;

  .frame {
    padding: 0px 40px;
    margin: 0 auto;
    min-width: 1024px;
    max-width: 1920px;
    box-sizing: border-box;

    .upper-frame {
      display: flex;

      .box-1 {
        display: flex;
        align-items: flex-start;
        flex: 2;
        justify-content: space-between;
        flex-direction: column;
        padding-left: 152px;

        .social-links {
          display: flex;
          flex-direction: row;
          font-size: 18px;
          margin-left: -23px;
          i {
            color: white;
          }
        }

        .logo-footer {
          margin-bottom: 64px;
          width: 301px;
          height: 199px;
        }
        .app-store {
          height: 40px;
          margin-right: 16px;
        }
        .google-play {
          height: 40px;
        }
      }
      .box-2,
      .box-3 {
        display: flex;
        flex-direction: column;
        flex: 1;
        margin-right: 207px;
        margin-top: 80px;

        .title-footer-section {
          line-height: 20px;
          margin-bottom: 24px;
          font-size: 16px;
          font-weight: bold;
        }
        a {
          color: #ffffff;
          text-decoration: none;
          line-height: 24px;
        }
        a:hover {
          text-decoration: underline;
        }
        ul {
          padding: 0;
          margin: 0;
          list-style: none;
        }
        li {
          display: block;
          margin-bottom: 16px;
        }
        .fa-language {
          color: white;
          margin-right: 3px;
        }
      }
    }
    .separate-line {
      margin: 40px 153px;
      background-color: #f6f6f6;
      border: none;
      height: 1px;
    }
    .bottom-frame {
      display: flex;
      justify-content: space-between;

      .social-links {
        display: flex;
        flex-direction: row;
        font-size: 18px;
        margin-left: -23px;
        i {
          color: white;
        }
      }
      .bottom-category {
        display: flex;
        flex-direction: row;

        a {
          color: white;
          text-decoration: none;
        }
      }
    }
    .bottom-line {
      color: white;
      margin-top: 10px;
      font-size: 13px;
      margin-left: auto;
      margin-right: auto;
      width: 200px;
    }
  }
}

@media screen and (max-width: 960px) {
  #nav {
    z-index: inherit;
    top: inherit;
    left: inherit;
    width: 100%;
    .inner-wrapper {
      padding: 0;
      display: flex;
      flex-direction: column;
      text-align: center;
    }
    a {
      color: white;
    }
  }

  .nav-links {
    display: flex;
    flex-direction: row;
    padding-left: 0px;
    margin-top: 0;
    margin-bottom: 0;
  }

  .nav-links li {
    padding-right: 25px;
    display: inherit;
    padding: 11px;
  }

  .nav-links li a {
    display: block;
    text-align: start; /* center avant*/
    padding: 20px 0;
    line-height: normal;
  }

  .separate-line-1 {
    margin: -20px 0px;
    margin-right: 35px;
    margin-left: 34px;
  }

  .banner {
    h1 {
      font-size: 32px;
      margin-top: 12rem;
    }
    h3 {
      font-size: 16px;
    }
  }
  .tarifs {
    padding-top: 3rem;
  }
  .footer {
    margin-top: 3rem;
    padding-top: 6rem;
    .frame {
      min-width: inherit;
      .upper-frame {
        flex-direction: column-reverse;
        .box-1 {
          padding-left: inherit;
          margin: auto;
          display: flex;
          flex-direction: column;
          margin-top: 2rem;
          .logo-footer {
            width: 150.5px;
            height: 99.5px;
            margin-bottom: 2rem;
          }
          .social-links {
            margin: 0;
            text-align: center;
          }
        }
        .box-3 {
          margin: auto;
          text-align: center;
        }
      }
      .separate-line {
        margin: 20px 105px;
      }
      .bottom-line {
        text-align: center;
      }
    }
  }
}
</style>
