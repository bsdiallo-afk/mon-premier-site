# CLAUDE.md

Ce fichier guide Claude Code (claude.ai/code) lorsqu'il travaille sur le code de ce dépôt.

## Projet

Un site statique d'une seule page pour se présenter, écrit en HTML et CSS simples. C'est un projet d'apprentissage : l'utilisateur débute en développement web.

Il n'y a ni étape de build, ni gestionnaire de paquets, ni linter, ni tests. Pour voir le site, il suffit d'ouvrir `index.html` dans un navigateur.

## Structure

- `index.html` contient tout le contenu de la page. Les liens du menu de l'en-tête mènent aux sections (`#apropos`, `#competences`, `#contact`) grâce à des ancres internes.
- `style.css` contient tous les styles. Les couleurs et la largeur maximale du contenu sont des variables CSS déclarées dans `:root` (`--couleur-accent`, etc.). Réutilisez-les avec `var(...)` au lieu d'écrire les valeurs en dur.
- La mise en page utilise flexbox pour l'en-tête, une grille CSS (`auto-fit`/`minmax`) pour les cartes de compétences, et un seul bloc `@media (max-width: 600px)` pour les téléphones.
- Les valeurs provisoires (« Votre Nom », `vous@exemple.com`) sont à remplacer par l'utilisateur.

## Conventions

- Le contenu du site, les noms de classes (`.entete`, `.carte`, `.bouton`, ...) et les commentaires du code sont en français. Gardez cette convention.
- Le code est volontairement simple et commenté pour faciliter l'apprentissage. N'ajoutez ni framework, ni outil de build, ni JavaScript sans que l'utilisateur le demande.
- Après chaque modification, expliquez-la en français, avec des mots accessibles à un débutant.
