# Atlas Communication 360° — site vitrine

Code source du site vitrine de l'agence **Atlas Communication 360°**, réalisé
exclusivement à partir de la charte graphique de la marque (couleurs orange
`#E86227` / jaune `#FFC919` / prune `#331832` / crème `#FFFAEB`, typographies
Fraunces + Montserrat).

## Hébergement

Le site de production est servi par **GitHub Pages**, depuis ce dépôt, sur
le nom de domaine personnalisé :

**https://atlas-communication-360.com**

(configuration : fichier `CNAME` à la racine + DNS chez le registrar pointant
vers GitHub Pages — voir Settings → Pages du dépôt).

Une version jumelle, éditable en direct depuis le navigateur, reste
disponible en tant qu'Artifact Claude :

**https://claude.ai/artifact/FMZpMnaWCjqXKQLwjYyN3L**

### Ajouter du contenu (réalisations, actualités)

Sur GitHub Pages, la page est **statique** : le panneau d'administration en
direct (qui republie la page depuis le navigateur) ne fonctionne que dans
l'Artifact Claude, pas ici. Pour ajouter ou modifier une réalisation ou une
actualité sur le site de production :

1. Éditer le tableau `SEED_DATA` (`portfolio` / `posts`) dans `index.html`
   (ou demander à Claude de le faire).
2. Committer et pousser sur `main` — GitHub Pages republie automatiquement
   en 1 à 2 minutes.

## SEO & responsive

- `index.html` est un document HTML5 complet et valide (`<!doctype>`, `<html lang="fr">`,
  `<head>` avec charset, viewport, meta description, balises Open Graph /
  Twitter Card, lien canonique, et un bloc JSON-LD `Organization` pour les
  moteurs de recherche).
- `robots.txt` + `sitemap.xml` déclarent le site aux robots d'indexation.
- `favicon.svg` / `favicon.ico` / `apple-touch-icon.png` / `icon-512.png` —
  déclinaisons de l'icône de marque pour onglets, favoris et écran d'accueil
  mobile.
- `og-image.png` (1200×630) — visuel utilisé pour les aperçus de partage sur
  les réseaux sociaux et la messagerie.
- La mise en page est responsive : navigation qui se replie en menu mobile,
  grilles qui passent de 3 à 2 puis 1 colonne selon la largeur d'écran, et un
  point de rupture dédié aux petits téléphones (< 480px) pour resserrer les
  espacements.

## Structure

- `CNAME` — nom de domaine personnalisé pour GitHub Pages.
- `.nojekyll` — désactive le traitement Jekyll (page statique pure).
- `index.html` — page unique contenant :
  - la navigation multi-pages (Accueil, L'agence, Services, Réalisations,
    Actualités, Contact) via un routeur par ancre (`#hash`) ;
  - tout le CSS et le JavaScript de la page ;
  - un espace d'administration intégré, actif uniquement sur l'Artifact
    Claude : toute personne connectée sur claude.ai avec les droits
    d'édition voit un mode édition lui permettant d'ajouter, modifier ou
    supprimer des **réalisations** et des **actualités** directement depuis
    la page. Sur GitHub Pages, ce panneau reste invisible pour tout le
    monde (comportement normal, pas un bug) : les visiteurs naviguent en
    lecture seule.

## Contact

- Email : contact@atlas-communication-360.com
- Instagram : [@Atlas_Communication_360](https://instagram.com/Atlas_Communication_360)
