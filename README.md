# Invitation Digitale — Didier & Diane

Invitation de mariage premium **Deux Cœurs, Une Destinée** — 20 Décembre 2030, Abomey-Calavi, Bénin.

## Stack

- HTML5
- CSS3 (variables, glassmorphism, motifs Africain chic)
- JavaScript Vanilla (modulaire)

## Structure

```
wedding-invitation/
├── index.html
├── assets/
│   ├── css/
│   │   ├── style.css
│   │   ├── animations.css
│   │   └── responsive.css
│   ├── js/
│   │   ├── main.js
│   │   ├── countdown.js
│   │   ├── music.js
│   │   ├── petals.js
│   │   ├── rsvp.js
│   │   └── gallery.js
│   ├── images/
│   ├── audio/
│   ├── video/
│   └── icons/
└── README.md
```

## Médias à déposer

Placez vos fichiers dans les dossiers correspondants. Le site fonctionne dès que les fichiers sont en place.

| Fichier | Chemin | Obligatoire |
|---------|--------|-------------|
| Vidéo splash | `assets/video/splash.mp4` | Recommandé |
| Photo couple | `assets/images/couple.jpg` | Oui (poster + fallback) |
| Hero | `assets/images/hero.jpg` | Oui |
| Marié | `assets/images/marie.jpg` | Oui |
| Mariée | `assets/images/mariee.jpg` | Oui |
| Galerie | `assets/images/gallery-1.jpg` … `gallery-6.jpg` | Oui |
| Fond cadeaux | `assets/images/gifts-bg.jpg` | Optionnel |
| Musique | `assets/audio/perfect-violoncelle.mp3` | Oui |

## Lancer le site

```bash
npx serve .
# ou
python -m http.server 8080
```

> Un serveur local est **recommandé** pour la vidéo splash et l’audio.

## EmailJS (RSVP)

1. Créez un compte sur [EmailJS](https://www.emailjs.com/)
2. Décommentez dans `index.html` :
   ```html
   <script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4/dist/email.min.js"></script>
   ```
3. Dans `assets/js/rsvp.js`, renseignez `serviceId`, `templateId`, `publicKey` et passez `enabled: true`

En attendant, les réponses sont enregistrées dans `localStorage` (clé `rsvp_responses`).

## Fonctionnalités

- Écran d’ouverture cinématique (vidéo + image fallback + effet lumière)
- Navigation sticky avec menu mobile et overlay
- Compte à rebours dynamique vers le 20 décembre 2030
- Sections : Union, Programme, Galerie (lightbox), Localisation, Cadeaux, RSVP, Contacts
- Musique Perfect (violoncelle) — **lecture manuelle uniquement**
- Pluie de pétales légère
- Animations scroll reveal
- Design responsive mobile / tablette / desktop

## Checklist de test

- [ ] Splash : vidéo ou fallback image, bouton « Entrer »
- [ ] Hero : parallaxe, panneau glass, badge cérémonie religieuse
- [ ] Compte à rebours : mise à jour chaque seconde
- [ ] Galerie : lightbox au clic (Escape pour fermer)
- [ ] RSVP : validation + message succès
- [ ] Musique : play/pause sans autoplay
- [ ] Mobile : menu hamburger, countdown 2×2
- [ ] Copie Mobile Money : toast de confirmation

## Couple


20 Décembre 2030 · Abomey-Calavi, Bénin
