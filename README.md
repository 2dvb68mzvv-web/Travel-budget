# Travel Budget — Dubaï 🇦🇪

Application web mobile, sans serveur et sans compte, pour estimer le budget de chaque voyageur.

## Installation sur GitHub Pages
1. Crée un dépôt public GitHub, par exemple `travel-budget`.
2. Ajoute **tous les fichiers de ce dossier à la racine** du dépôt (`index.html`, `style.css`, `app.js`, `manifest.webmanifest`, `icon.svg`).
3. Dans **Settings → Pages**, choisis **Deploy from a branch**, branche **main**, dossier **/(root)** puis **Save**.
4. Ouvre l'URL affichée par GitHub Pages dans Safari sur iPhone.
5. Dans Safari, utilise **Partager → Sur l'écran d'accueil**.

## Personnalisation des catalogues
Les listes `ACT` et `FOOD` sont au début de `app.js`. Chaque entrée est sous la forme `["Nom", prix_en_euros]`.

## Données
Les informations sont enregistrées via `localStorage` sur chaque navigateur/appareil. Aucun compte, aucune synchronisation, aucun serveur. Effacer les données du site peut effacer le budget. Les prix du catalogue sont des références fournies par l'organisateur et non des tarifs garantis. L'heure d'arrivée est interprétée dans le fuseau de Dubaï UTC+4.

## Comptabilité
Le montant « Économies disponibles » représente l'argent **encore disponible**, pas les versements historiques déjà utilisés pour payer l'avion ou l'hôtel. Quand un voyageur coche un paiement, il doit mettre à jour son épargne disponible si celle-ci a servi à régler ce paiement, afin d'éviter un double comptage.
