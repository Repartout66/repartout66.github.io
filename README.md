# Repartout66 — Site vitrine

Site vitrine statique (HTML/CSS/JS) pour la boutique de dépannage informatique Repartout66.

## Contenu

- `index.html` — page d'accueil (présentation, prestations)
- `pihole.html` — page dédiée à l'explication et à l'installation du Pi-Hole
- `contact.html` — page de contact avec formulaire
- `confidentialite.html` — page de confidentialité / RGPD (accessible depuis le pied de page de chaque page)
- `style.css` — feuille de style unique du site

Aucune dépendance à installer : c'est du HTML/CSS/JS pur, compatible avec GitHub Pages tel quel.

## Formulaire de contact (Formspree)

Le formulaire de `contact.html` est déjà relié à votre formulaire Formspree (`https://formspree.io/f/mrpbbzpk`). Formspree vous enverra un email de confirmation lors du tout premier envoi : validez-le pour activer la réception des demandes.

## Déploiement sur GitHub Pages

Le dépôt prévu est `https://github.com/MoraruLeQuag/repartout.github.io`.

1. Créez le dépôt sur GitHub avec exactement ce nom (`repartout.github.io`) s'il n'existe pas déjà.
2. Placez les fichiers de ce dossier (`index.html`, `pihole.html`, `contact.html`, `confidentialite.html`, `style.css`, `README.md`) à la racine du dépôt.
3. Poussez-les sur la branche `main` :
   ```bash
   git init
   git remote add origin https://github.com/MoraruLeQuag/repartout.github.io.git
   git add .
   git commit -m "Site vitrine Repartout66"
   git branch -M main
   git push -u origin main
   ```
4. Dans les paramètres du dépôt GitHub (**Settings > Pages**), vérifiez que la source est bien la branche `main` et le dossier `/root`.
5. Le site sera accessible à l'adresse `https://moraruLeQuag.github.io` (ou l'URL indiquée par GitHub Pages) après quelques minutes.

## Personnalisation rapide

- **Couleurs** : modifiables dans les variables en haut de `style.css` (`--blue`, `--green`, etc.).
- **Prestations** : chaque service est une `<article class="service-card">` dans `index.html`, facile à dupliquer ou modifier.
- **Photo de profil** : le badge rond "G" dans la section "Qui suis-je" peut être remplacé par une vraie photo en changeant le contenu de `.about-badge` dans `index.html`.
