# Memory
# Jeu du Memory

Un jeu de Memory interactif, rapide et responsive développé en **HTML5**, **CSS3** et **JavaScript** (Vanilla).

---

## Présentation du projet

Le but du jeu est de retrouver toutes les paires d'images identiques dissimulées derrière les cartes en réalisant le moins de coups possible et dans le temps le plus court.

### Fonctionnalités
- **Génération dynamique des cartes** : Les images sont récupérées aléatoirement à chaque partie via l'API [Picsum Photos](https://picsum.photos/).
- **Mélange aléatoire** : Implémentation de l'algorithme de mélange Fisher-Yates pour redistribuer les cartes à chaque nouvelle partie.
- **Compteur de coups et chronomètre** : Suivi en direct du nombre d'essais et du temps écoulé.
- **Gestion des contrôles** : Boutons *Démarrer* et *Recommencer* gérant dynamiquement l'état et la réinitialisation de la partie.
- **Accessibilité** : Utilisation d'attributs ARIA (`role="button"`, `tabindex="0"`, `aria-live="polite"`) pour une meilleure accessibilité.

---

## Design & Style (CSS)

Le style de l'interface a été conçu pour être épuré, agréable et ergonomique :
- Disposition fluide du plateau avec **CSS Flexbox**.
- Effets d'ombrage et dégradés modernes pour l'aspect des cartes.
- **Inspirations de templates** : Pour la structure visuelle et les idées de style (notamment l'en-tête et les composants d'interface), différents templates ont été explorés et adaptés depuis [FreeFrontend - CSS Headers](https://freefrontend.com/css-headers/#examples).

---

## Structure des fichiers

```text
├── index.html    # Structure sémantique du jeu et de l'interface
├── style.css     # Mise en page, styles des cartes et des contrôles
├── memory.js     # Logique du jeu (tirage, minuterie, gestion des clics et paires)
└── README.md     # Documentation du projet
