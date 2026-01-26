<script setup>
import { ref } from 'vue'

const hebergements = ref([
  {
    id: 1,
    nom: 'O PANIER DE ROSES',
    adresse: 'Saint Nizier D’Azergues',
    tel: '06.80.60.34.27',
    description: 'Gite 9/11 personnes',
    distance: '12 minutes',
    site: 'https://www.airbnb.fr/rooms/35422861?source_impression_id=p3_1769007182_P3_nineVllY9T0Ax&check_in=2026-08-29&guests=1&adults=1&check_out=2026-08-30'
  },
  {
    id: 2,
    nom: 'Gite La Muzetiere',
    adresse: 'Chamelet',
    tel: '07.57.54.00.78',
    description: 'Gite et chambres cabanes eco-conçues',
    distance: '6 minutes',
    site: 'https://la-muzetiere.fr/',
    airbnb1: 'https://www.airbnb.fr/rooms/893501501341087899?adults=1&children=0&infants=0&pets=0&wishlist_item_id=11005835739470&check_in=2026-08-29&check_out=2026-08-30&source_impression_id=p3_1769288630_P3_dDrD58oVCPRQb&previous_page_section_name=1001',
    airbnb2: 'https://www.airbnb.fr/rooms/638229309053391135?adults=1&children=0&infants=0&pets=0&wishlist_item_id=11005835729470&check_in=2026-08-29&check_out=2026-08-30&source_impression_id=p3_1769288648_P3IqYoGy93Joji3k&previous_page_section_name=1001',
  },
  {
    id: 3,
    nom: 'Entre couette et bulles',
    adresse: 'Rivolet',
    description: 'Chalets au coeur du Beaujolais',
    distance: '18 minutes',
    site: 'https://entre-couette-et-bulles.com/chalets/',
    airbnb1: 'https://www.airbnb.fr/rooms/1401476589115469891?adults=1&children=0&infants=0&pets=0&wishlist_item_id=11005835859747&check_in=2026-08-29&check_out=2026-08-30&source_impression_id=p3_1769289481_P3kee_3ooQIzGFE3&previous_page_section_name=1001',
    airbnb2: 'https://www.airbnb.fr/rooms/1325889070938877914?adults=1&children=0&infants=0&pets=0&wishlist_item_id=11005835861786&check_in=2026-08-29&check_out=2026-08-30&source_impression_id=p3_1769289636_P3h89tIh-HzVfv1q&previous_page_section_name=1001'
  },
  {
    id: 4,
    nom: 'Gite l’Orée du Bois',
    adresse: 'Ternand',
    tel: '06 83 56 96 67',
    description: 'Chez Michelle et Michel - Possibilité d’arriver aux domaine en calèche (LOL)',
    distance: '15 minutes',
    site: 'https://www.gite-beaujolais-randonnee-attelage.fr/',
  },
  {
    id: 5,
    nom: 'Appartement meublé touristique',
    adresse: 'Chamelet',
    tel: '06 83 56 96 67',
    description: 'Jusqu\'à 6 personnes',
    distance: '6 minutes',
    airbnb1: 'https://www.airbnb.fr/rooms/1267309711251449531?adults=8&children=0&infants=0&pets=0&wishlist_item_id=11005835738606&check_in=2026-08-29&check_out=2026-08-30&source_impression_id=p3_1769417742_P3WZJsZUdAbM6_d8&previous_page_section_name=1000',
  },
  {
    id: 6,
    nom: 'Chambres d’hôtes « C Naturel »',
    adresse: 'Dieme',
    tel: '06.31.06.20.50',
    distance: '15 minutes',
    site: 'https://cnaturel.ellohaweb.com/',
  },
  {
    id: 7,
    nom: 'La Batisse des tuileries côté forêt',
    adresse: 'Lamures-sur-Azergues',
    description: 'Jusqu\'à 10 personnes',
    tel: '06.31.06.20.50',
    distance: '8 minutes',
    airbnb1: 'https://www.airbnb.fr/rooms/1581989043081549349?adults=1&children=0&infants=0&pets=0&wishlist_item_id=11005835741030&check_in=2026-08-29&check_out=2026-08-30&source_impression_id=p3_1769289207_P36jQ4OyzusBHEEe&previous_page_section_name=1001',
  },
  {
    id: 8,
    nom: 'Azergues plaisir de vivre',
    adresse: 'Grandris',
    description: 'Chambre d\'hotes',
    tel: '06 80 54 17 57 ou 04.74.66.82.28',
    distance: '15 minutes',
    site: 'https://www.beaujolaisvert.com/prestataire/azergues-le-plaisir-de-vivre-374349/',
  },
  {
    id: 9,
    nom: 'L’évasion entre prairies et forêts',
    adresse: 'Lamures-sur-Azergues',
    description: 'Gite pour 6 personnes',
    tel: '06 24 10 25 92',
    distance: '8 minutes',
    site: 'https://www.beaujolaisvert.com/prestataire/levasion-entre-prairie-et-forets-73861-6041650/',
  },
  {
    id: 10,
    nom: 'Studio au petit midi ',
    adresse: 'Saint Just d’Avray',
    description: 'Pour 2 personnes',
    distance: '35 minutes',
    airbnb1: 'https://www.airbnb.fr/rooms/1388458100484352875?adults=8&children=0&infants=0&pets=0&wishlist_item_id=11005835863007&check_in=2026-08-29&check_out=2026-08-30&source_impression_id=p3_1769417742_P3mDq11AlQrFq-K7&previous_page_section_name=1000',
  },
  {
    id: 11,
    nom: 'Gite Le Géode',
    adresse: 'Saint Cyr le Chatoux',
    description: 'Pour 3 personnes',
    tel: '',
    distance: '15 minutes',
    airbnb1: 'https://www.airbnb.fr/rooms/1394869517173205989?adults=8&children=0&infants=0&pets=0&wishlist_item_id=11005835860984&check_in=2026-08-29&check_out=2026-08-30&source_impression_id=p3_1769417742_P3UahE4Q5wD3ElRs&previous_page_section_name=1000',
  },
  {
    id: 12,
    nom: 'Domaine Dumas',
    adresse: 'Ternand',
    description: 'Chambres d’hôtes (jusqu’à 9 personnes)',
    tel: '06.83.32.69.21',
    distance: '15 minutes',
    site: 'https://www.gites-de-france-rhone.com/location-vacances-Chambre-d-hotes-Ternand-69G2200.html',
  },
  {
    id: 13,
    nom: 'Gites Domaine des Mollières',
    adresse: 'Grandris',
    description: '15 couchages',
    tel: '04 74 60 13 59',
    distance: '15 minutes',
    site: 'https://www.domainedesmollieres.com/le-domaine',
  },
  {
    id: 14,
    nom: 'Domaine de la Poyat',
    adresse: 'Legny',
    description: 'gite pour personnes a mobilites reduites',
    tel: '06 85 13 02 00',
    distance: '18 minutes',
    site: 'https://www.domainedelapoyat.fr/hote.html',
  },
  {
    id: 15,
    nom: 'Gîte chez le Vigneron',
    adresse: 'Ternand',
    description: 'Gite 8 personnes',
    tel: '06.80.27.03.67',
    distance: '15 minutes',
    site: 'https://www.gites-de-france-rhone.com/location-vacances-Gite-a-Ternand-Rhone-69G1752.html',
  },
  {
    id: 16,
    nom: 'Camping Le Lyzeron',
    adresse: 'Lamure-sur-azergues',
    description: 'Pour camper',
    tel: '07.87.77.50.03',
    distance: '10 minutes',
    site: 'https://www.campinglelyzeron.com/',
  },
  {
    id: 17,
    nom: 'Sandrine et Jean - 10pers',
    adresse: 'Chambost-Allières',
    description: 'Gite conseillé par les propriétaires du domaine',
    tel: '07 83 98 19 29',
    distance: '7 minutes',
  },
  {
    id: 18,
    nom: 'Martine Mousset - 8 pers',
    adresse: 'Lamure-sur-azergues',
    description: 'Gite conseillé par les propriétaires du domaine',
    tel: '06 37 66 96 95',
    distance: '8 minutes',
  },
  {
    id: 19,
    nom: 'Faustine et Ludo Pernoud - 4 pers',
    adresse: 'Chambost-Allières',
    description: 'Gite conseillé par les propriétaires du domaine',
    tel: '06 59 30 06 39',
    distance: '7 minutes',
  }
])
</script>

<template>
  <div class="page">
    <img src="/src/assets/lovers.png" alt="" class="lovers-img" />

    <header class="hero">
      <h1>Chloé & Rémi</h1>
      <p class="date">• 29 Août 2026 • </p>
    </header>

    <section class="intro">
      <h2>Bienvenue</h2>
      <p>
        Nous sommes très heureux de partager cette journée avec vous 💍
      </p>
      <p>
        Vous trouverez ci-dessous une sélection de lieux d’hébergement à proximité du lieu de réception.
      </p>

      <p>
        <strong>
          Cette liste de logements proches du domaine n’est pas exhaustive ! Elle recense les
          adresses les plus proches et/ou conseillées par les propriétaires du Domaine. Ne pas
          hésiter à consulter Airbnb, en regardant jusqu’à Vaux en Beaujolais / Le Perréon (18
          minutes du Domaine) ou encore Saint Just D’Avray (35 minutes du Domaine).
        </strong>
      </p>
    </section>

    <section class="hebergements">
      <h2>Hébergements à proximité</h2>
      <ul class="list">
        <li v-for="lieu in hebergements" :key="lieu.id" class="card">
          <h3>{{ lieu.nom }}</h3>
          <p class="adresse">{{ lieu.adresse }}</p>
          <p>{{ lieu.description }}</p>
          <p>{{ lieu.tel }}</p>
          <p class="distance">📍 {{ lieu.distance }}</p>
          <a v-if="lieu.site" :href="lieu.site" target="_blank" rel="noopener">
            Voir le site
          </a>
          
          <a v-if="lieu.airbnb1" :href="lieu.airbnb1" target="_blank" rel="noopener">
            Airbnb
          </a>
          
          <a v-if="lieu.airbnb2" :href="lieu.airbnb2" target="_blank" rel="noopener">
            Airbnb
          </a>
        </li>
      </ul>
    </section>

    <div class="event-date">
      <p>Le Samedi 29 août 2026 à 15h30</p>
    </div>

    <div class="address">
      <p>Au Domaine de Montfriol</p>
      <p>10 Route de l'Azergues</p>
      <p>69870 Chambost-Allières</p>
    </div>

    <footer class="footer">
      <p>Merci et à très bientôt ❤️</p>
    </footer>
  </div>
</template>

<style scoped>
.page {
  position: relative;
  font-family: "Cormorant Garamond", system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  max-width: 900px;
  margin: 0 auto;
  font-style: italic;
  color: #000000;
}

.lovers-img {
  position: absolute;
  top: -20px;
  left: -20px;
  height: 200px;

  @media only screen and (max-width: 576px) {
    height: 100px;
  }
}

.hero {
  text-align: center;
  margin-bottom: 2rem;
}

.hero h1 {
  font-family: "Great Vibes", cursive;
  font-size: 2.5rem;
  margin-bottom: 0.5rem;
  color: #ff6445;

  @media only screen and (max-width: 576px) {
    font-size: 2rem;
  }
}

.hebergements p {
  margin: 0;
}

.date {
  font-style: italic;
  color: #777;
}

section {
  margin-bottom: 2rem;
}

.list {
  list-style: none;
  padding: 0;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1rem;
}

.card {
  border: 1px solid #e5e5e5;
  border-radius: 8px;
  padding: 0.5rem;
  background: #fafafa;
}

.card h3 {
  margin: 0;
}

.adresse {
  font-size: 0.9rem;
  color: #666;
  padding-bottom: 20px;
}

.distance {
  font-size: 0.9rem;
  margin-top: 0.5rem;
}

.card a {
  display: block;
  margin-top: 0.5rem;
  color: #b76e79;
  text-decoration: none;
  font-weight: 500;
}

.card a:hover {
  text-decoration: underline;
}

.event-date {
  font-size: 1.5rem;
  font-family: "Great Vibes", cursive;
  /* line-height: 20px; */
  color: #ff6445;

  p {
    margin: 0;
  }
}

.address {
  p {
    margin: 0;
  }
}

.footer {
  color: #777;
  text-align: center;
  margin-top: 3rem;
}
</style>
