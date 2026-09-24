# Atlas Communication 360° — site vitrine

Code source du site vitrine de l'agence **Atlas Communication 360°**, réalisé
exclusivement à partir de la charte graphique de la marque (couleurs orange
`#E86227` / jaune `#FFC919` / prune `#331832` / crème `#FFFAEB`, typographies
Fraunces + Montserrat).

## Hébergement

Le site est **hébergé et édité en direct** en tant qu'Artifact Claude :

**https://claude.ai/artifact/FMZpMnaWCjqXKQLwjYyN3L**

Ce dépôt Git ne sert pas à l'hébergement du site : c'est une copie de
sauvegarde et de versioning du code source (`index.html`, fichier unique,
sans dépendance de build). Pour toute modification, éditer ce fichier et le
republier sur claude.ai (ou demander à Claude de le faire), puis pousser la
même version ici pour garder l'historique à jour.

## Structure

- `index.html` — page unique contenant :
  - la navigation multi-pages (Accueil, L'agence, Services, Réalisations,
    Actualités, Contact) via un routeur par ancre (`#hash`) ;
  - tout le CSS et le JavaScript de la page ;
  - un espace d'administration intégré : toute personne connectée sur
    claude.ai avec les droits d'édition sur l'Artifact voit un mode édition
    lui permettant d'ajouter, modifier ou supprimer des **réalisations** et
    des **actualités** directement depuis la page. Chaque sauvegarde republie
    le site pour tous les visiteurs.
  - Les visiteurs normaux (sans droits d'édition) ne voient jamais ces
    contrôles : ils naviguent en lecture seule.

## Contact

- Email : contact@atlas-communication-360.com
- Instagram : [@Atlas_Communication_360](https://instagram.com/Atlas_Communication_360)
