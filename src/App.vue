<template>
  <div class="page">
    <header class="hero">
      <h1>Marie & Julien</h1>
      <p class="date">12 juillet 2026 • Bordeaux</p>
    </header>

    <section class="intro">
      <h2>Bienvenue</h2>
      <p>
        Nous sommes très heureux de partager cette journée avec vous 💍
        Vous trouverez ci-dessous une sélection de lieux d’hébergement à proximité du lieu de réception.
      </p>
    </section>

    <section class="hebergements">
      <h2>Hébergements à proximité</h2>
      <ul class="list">
        <li v-for="lieu in hebergements" :key="lieu.id" class="card">
          <h3>{{ lieu.nom }}</h3>
          <p class="adresse">{{ lieu.adresse }}</p>
          <p>{{ lieu.description }}</p>
          <p class="distance">📍 {{ lieu.distance }}</p>
          <a v-if="lieu.site" :href="lieu.site" target="_blank" rel="noopener">
            Voir le site
          </a>
        </li>
      </ul>
    </section>

    <footer class="footer">
      <p>Merci et à très bientôt ❤️</p>
    </footer>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const hebergements = ref([
  {
    id: 1,
    nom: 'Hôtel du Parc',
    adresse: '10 rue des Fleurs, Bordeaux',
    description: 'Hôtel confortable avec petit-déjeuner inclus.',
    distance: '5 minutes en voiture',
    site: 'https://example.com'
  },
  {
    id: 2,
    nom: 'Maison d’hôtes La Roseraie',
    adresse: '25 chemin des Vignes, Pessac',
    description: 'Charmante maison d’hôtes au calme.',
    distance: '8 minutes en voiture',
    site: ''
  },
  {
    id: 3,
    nom: 'Gîte des Chênes',
    adresse: 'Route de Léognan',
    description: 'Gîte idéal pour les familles ou groupes d’amis.',
    distance: '12 minutes en voiture',
    site: ''
  }
])
</script>

<style scoped>
.page {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  max-width: 900px;
  margin: 0 auto;
  padding: 1.5rem;
  color: #333;
}

.hero {
  text-align: center;
  margin-bottom: 2rem;
}

.hero h1 {
  font-size: 2.5rem;
  margin-bottom: 0.5rem;
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
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
}

.card {
  border: 1px solid #e5e5e5;
  border-radius: 8px;
  padding: 1rem;
  background: #fafafa;
}

.card h3 {
  margin-top: 0;
}

.adresse {
  font-size: 0.9rem;
  color: #666;
}

.distance {
  font-size: 0.9rem;
  margin-top: 0.5rem;
}

.card a {
  display: inline-block;
  margin-top: 0.5rem;
  color: #b76e79;
  text-decoration: none;
  font-weight: 500;
}

.card a:hover {
  text-decoration: underline;
}

.footer {
  text-align: center;
  margin-top: 3rem;
  color: #777;
}
</style>
