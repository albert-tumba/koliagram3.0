<template>
  <div class="wrapper-cm">
    <h1>Community Mangement 👨‍💻</h1>
    <div class="inner-wrapper-cm">
      <div class="text-area">
        <h3>Gestion de vos réseaux sociaux</h3>
        <p>
          Nous publions du contenu sur vos réseaux au rythme que vous souhaitez
          (généralement tous les jours, deux jours ou quatre jours). Les
          contenus postés sont visuellement attractif afin d'obtenir le plus
          grand nombre de j'aimes possible. Les stories Instagram sont également
          comprises dans nos prestations et permettent de garder la page la plus
          active possible.
        </p>
      </div>
      <div class="image-area">
        <img src="@/assets/social.png" class="img-1" />
      </div>
    </div>

    <div class="inner-wrapper-cm-2">
      <div class="image-area-2">
        <img src="@/assets/sponso.png" class="img-2" />
      </div>
      <div class="text-area-2">
        <h3>Sponsorisations</h3>
        <p>
          Les jeux concours nous permettent d'agrandir et de fidéliser votre
          communauté en leur offrant quelque chose à gagner. Les sponsorisations
          agrandissent votre communauté, car les abonnés de votre page Instagram
          ou Facebook vont inviter d'autres amis à voir la publication (en les
          taggant) afin d'augmenter leurs chances de gagner à votre jeu
          concours. Par cette opération, vous gagner en visibilité et votre
          communauté s'agrandit.
        </p>
      </div>
    </div>

    <div class="inner-wrapper-cm-3">
      <div class="text-area-3">
        <h3>Modération des commentaires et réponses aux messages privés</h3>
        <p>
          Nous modérons les commentaires sous les publications afin d'éviter
          tous commentaires négatifs. Cela nous permet également d'interagir
          avec votre communauté et de les maintenir engagés sur la page. Nous
          répondons aussi aux messages privés afin que chacun de vos clients ait
          une réponse rapide à leurs interrogations.
        </p>
      </div>
      <div class="image-area-3">
        <img src="@/assets/moderation.png" class="img-3" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CM",
};
</script>

<style scoped lang="scss">
.wrapper-cm {
  margin-left: auto;
  margin-right: auto;
  width: 1035px;
  font-family: "Roboto", sans-serif;
  h1 {
    font-size: 30px;
    text-align: center;
  }
  h3 {
    text-align: start;
  }
}

.communitymanagement {
  background-color: #f7f9fc;
}
.communitymanagement {
  padding: 2em;
}

.inner-wrapper-cm {
  display: flex;
  flex-direction: row;
  padding-top: 3em;
  padding-bottom: 4em;
  .text-area {
    margin-right: 6.5rem;
    text-align: start;
    padding-top: 1rem;

    h3 {
      font-size: 32px;
      font-weight: bold;
    }
  }
  p {
    font-weight: bold;
  }
  .image-area {
    .img-1 {
      border-radius: 8px;
    }
  }
}

.inner-wrapper-cm-2 {
  display: flex;
  flex-direction: row;
  padding-top: 2em;
  padding-bottom: 4em;
  .text-area-2 {
    margin-left: 6.5rem;
    padding-top: 1rem;
    h3 {
      font-size: 32px;
      font-weight: bold;
    }
  }
  .img-2 {
    width: 500px;
    height: 357.14px;
    border-radius: 8px;
  }
}

.inner-wrapper-cm-3 {
  display: flex;
  flex-direction: row;
  padding-top: 2em;
  padding-bottom: 4em;
  .text-area-3 {
    margin-right: 6.5rem;
    padding-top: 1em;
    h3 {
      font-size: 32px;
      font-weight: bold;
    }
  }
  .img-3 {
    width: 500px;
    height: 357.14px;
    border-radius: 8px;
  }
}

@media screen and (max-width: 960px) {
  .wrapper-cm {
    width: 100%;
    h1 {
      font-size: 26px;
    }
  }
  .inner-wrapper-cm {
    display: flex;
    flex-direction: column;
    padding-top: 0;
    padding-bottom: 2rem;
    .text-area {
      margin-right: auto;
      margin-left: auto;
      padding-top: 0rem;
      width: 285px;
      h3 {
        font-size: 17px;
        text-align: center;
      }
      p {
        font-size: 12px;
        text-align: justify;
      }
    }
    .image-area {
      text-align: center;
      .img-1 {
        width: 291.6px;
        height: 208.3px;
      }
    }
  }

  .inner-wrapper-cm-2 {
    display: flex;
    flex-direction: column-reverse;
    padding-top: 1rem;
    .text-area-2 {
      margin-right: auto;
      margin-left: auto;
      padding-top: 0;
      width: 285px;
      h3 {
        font-size: 17px;
        text-align: center;
      }
      p {
        font-size: 12px;
        text-align: justify;
      }
    }
    .image-area-2 {
      text-align: center;
      .img-2 {
        width: 291.6px;
        height: 208.3px;
      }
    }
  }

  .inner-wrapper-cm-3 {
    display: flex;
    flex-direction: column;
    padding-top: 0;
    padding-bottom: 2rem;
    .text-area-3 {
      margin-right: auto;
      margin-left: auto;
      padding-top: 0rem;
      width: 285px;
      h3 {
        font-size: 17px;
        text-align: center;
      }
      p {
        font-size: 12px;
        text-align: justify;
      }
    }
    .image-area-3 {
      text-align: center;
      .img-3 {
        width: 291.6px;
        height: 208.3px;
      }
    }
  }
}
</style>