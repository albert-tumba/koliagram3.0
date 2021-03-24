<template>
  <div class="wrapper-tarifs">
    <h1>Tarifs 💰</h1>
    <h3>On vous simplifie la vie, au meilleur prix !</h3>
    <div class="inner-wrapper-tarifs">
      <div class="pricing-section">
        <div class="pricing-table">
          <div class="pricing-card">
            <h3 class="pricing-card-header">Initial</h3>
            <div class="price">200<span>€/Mois</span></div>
            <ul>
              <li>Publications 3 fois par semaine sur Instagram et Facebook</li>
              <li>Réponse aux messages privés sous 1h</li>
              <li>Réponse aux avis Google My Business</li>
            </ul>
            <a href="#" class="order-btn">En savoir plus</a>
          </div>

          <div class="pricing-card">
            <h3 class="pricing-card-header">Standard</h3>
            <div class="price">300<span>€/Mois</span></div>
            <ul>
              <li>Publications 5 fois par semaine sur Instagram et Facebook</li>
              <li>Séance photo toutes les 4 semaines</li>
              <li>Organisation/Montage photo pour jeu concours</li>
              <li>Réponse aux messages privés sous 1h</li>
              <li>Réponse aux avis Google My Business</li>
            </ul>
            <a href="#" class="order-btn">En savoir plus</a>
          </div>

          <div class="pricing-card pricing-card-3">
            <h3 class="pricing-card-header">Premium</h3>
            <div class="price">400<span>€/Mois</span></div>
            <ul>
              <li>Publications 7 fois par semaine sur Instagram et Facebook</li>
              <li>Séance photo toutes 4 les semaines</li>
              <li>Organisation/Montage photo pour jeu concours</li>
              <li>Réponse aux messages privés sous 1h</li>
              <li>Réponse aux avis Google My Business</li>
              <li>Réponse aux avis Ubereats</li>
              <li>Gestion des relations avec les influenceurs</li>
            </ul>
            <a href="#" class="order-btn">En savoir plus</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Pricing",
};
</script>

<style scoped>
* {
  text-decoration: none;
  list-style: none;
}
.wrapper-tarifs {
  margin-left: auto;
  margin-right: auto;
  width: 1035px;
}

.wrapper-tarifs h1 {
  font-size: 30px;
  text-align: center;
}

.wrapper-tarifs h3 {
  font-size: 17px;
  text-align: center;
}

.pricing-section {
  height: 100vh;
  margin-top: 3em;
}

.intro-pricing h1 {
  font-size: 30px;
  font-weight: bold;
}

.intro-pricing h2 {
  font-size: 15px;
  font-weight: lighter;
}

.pricing-table {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  justify-content: space-around;
  width: min(1600px, 100%); /* px et % pose problème pour le SCSS */
  margin: auto;
  margin-top: Opx;
}

.pricing-card {
  flex: 1;
  max-width: 360px;
  background-color: #fff;
  margin: 0px 12px;
  text-align: center;
  cursor: pointer;
  overflow: hidden;
  color: #2d2d2d;
  transition: 0.3s linear;
  border-radius: 8px;
  box-shadow: 0 15px 35px rgba(50, 50, 93, 0.1);
}

.pricing-card-header {
  background-color: #f7963e;
  display: inline-block;
  color: #fff;
  padding: 12px 30px;
  border-radius: 0 0 20px 20px;
  font-size: 16px;
  text-transform: uppercase;
  font-weight: 600;
  transition: 0.4s linear;
}

.pricing-card:hover .pricing-card-header {
  box-shadow: 0 0 0 5em #f7963e;
}

.pricing-card ul {
  padding: 5px;
}

.price {
  font-size: 35px;
  color: #f7963e;
  margin: 20px 0;
  transition: 0.2s linear;
}

.price span {
  font-size: 22px;
  font-weight: 700;
}

.pricing-card:hover {
  color: black;
}
.pricing-card:hover .price {
  color: #fff;
}

.pricing-card li {
  font-size: 16px;
  padding: 10px 0;
}

.order-btn {
  display: inline-block;
  margin-bottom: 20px;
  border: 2px solid #f7963e;
  color: #f7963e;
  padding: 8px 20px;
  border-radius: 50px;
  font-weight: 500;
  transition: 0.3s linear;
  margin-bottom: 3em;
  margin-top: 1.5em;
}

.order-btn:hover {
  background-color: #f7963e;
  color: #fff;
  text-decoration: none;
}

@media screen and (max-width: 1100px) {
  .wrapper-tarifs {
    width: inherit;
  }

  .pricing-section {
    height: inherit;
  }
  .pricing-table {
    display: flex;
    flex-direction: column;
    width: inherit;
  }
  .pricing-card {
    margin-bottom: 1.5rem;
  }
}
</style>