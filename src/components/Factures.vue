<template>
  <div class="wrapper-factures">
    <h1>Factures 🧾</h1>
    <h2>Prix fixe : 99,90€ par commerce.</h2>
    <div class="inner-wrapper-factures">
      <div class="text-area">
        <h3>Simplifier au maximum la récupération de vos factures</h3>
        <p>
          Nous procédons à la collecte automatique de vos factures sur vos
          espaces clients professionnels ainsi que sur vos boîtes mails
          professionnelles. Nous mettons également en place une conversation
          Whatsapp avec vos équipes sur place afin qu'ils nous transmettent via
          une simple photos les justificatifs de paiements qu'ils auraient
          effectué pour votre commerce. 3. Vos factures sont sauvegardées sur un
          espace en ligne sécurisé, accessible uniquement par vous et nous.
        </p>
      </div>
      <div class="image-area">
        <img src="@/assets/invoices.jpeg" class="img-4" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Factures",
};
</script>

<style scoped lang="scss">
.wrapper-factures {
  margin-left: auto;
  margin-right: auto;
  width: 1035px;
  h1 {
    font-size: 30px;
    text-align: center;
  }
  h2 {
    font-size: 17px;
    text-align: center;
  }
}

.inner-wrapper-factures {
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
    .img-4 {
      border-radius: 8px;
      width: 500px;
      height: 357.14px;
    }
  }
}

@media screen and (max-width: 960px) {
  .wrapper-factures {
    width: 100%;
    h1 {
      font-size: 26px;
      text-align: center;
    }
    h2 {
      font-size: 17px;
      text-align: center;
    }
  }

  .inner-wrapper-factures {
    display: flex;
    flex-direction: column;
    padding-top: 0;
    padding-bottom: 4em;
    .text-area {
      margin-right: auto;
      margin-left: auto;
      padding-top: 0rem;
      width: 265px;
      h3 {
        font-size: 16px;
        font-weight: bold;
        text-align: center;
      }
    }
    p {
      font-size: 12px;
      font-weight: bold;
      text-align: justify;
    }
    .image-area {
      text-align: center;
      .img-4 {
        width: 267.08px;
        height: 190.775px;
      }
    }
  }
}
</style>