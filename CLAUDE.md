# Conventions

- Tout tient dans `index.html` (HTML, CSS, JS, aucune dépendance) : le fichier doit fonctionner hors ligne, ouvert directement.
- Interface en français, droit au but : le résultat se calcule pendant la saisie, pas de texte d'explication.
- Bouton mode clair / mode sombre dans la barre du haut (choix enregistré dans le navigateur) ; toute couleur passe par les variables CSS de `:root`.

# Ajouter un calculateur

1. Ajouter une `<section class="tool" id="..." data-tab="Nom de l'onglet">` dans `<main>` ; l'onglet est créé automatiquement.
2. Ajouter son script (une IIFE) à la fin, en réutilisant `num`, `fmt`, `store` et les classes `card`, `fields`, `field`, `inp`, `results`, `res`, `chip`.
3. Un champ avec `data-save="clé"` est mémorisé automatiquement (réglages seulement, pas les valeurs patient).
