# Ohmyfood

Ohmyfood est un site web pour découvrir et commander des plats de restaurants. Ce projet met en avant l'utilisation d'animations CSS, de techniques de design responsive et de bonnes pratiques de développement web.

## Table des matières
- [Ohmyfood](#ohmyfood)
  - [Table des matières](#table-des-matières)
  - [Aperçu](#aperçu)
  - [Fonctionnalités](#fonctionnalités)
  - [Technologies utilisées](#technologies-utilisées)
  - [Installation](#installation)
  - [Utilisation](#utilisation)
  - [Structure du projet](#structure-du-projet)
  - [Animations et choix techniques](#animations-et-choix-techniques)
    - [Animation du cœur](#animation-du-cœur)
    - [Sélecteur de plat](#sélecteur-de-plat)
    - [Choix des animations](#choix-des-animations)
    - [Conception mobile first](#conception-mobile-first)
  - [Auteur](#auteur)

## Aperçu

Ohmyfood permet aux utilisateurs de visualiser les menus de différents restaurants et de passer des commandes. Chaque restaurant a une page dédiée avec des animations pour les éléments interactifs.

## Fonctionnalités

- Affichage des menus de restaurants avec des animations.
- Sélecteur de plats interactif.
- Animation de cœur pour ajouter des restaurants aux favoris.
- Design responsive adapté aux mobiles et aux tablettes.

## Technologies utilisées

- HTML
- CSS
- JavaScript
- Font Awesome pour les icônes
- Google Fonts pour la typographie

## Installation

Pour installer et exécuter ce projet localement, suivez ces étapes :

1. Clonez le repository :
   ```bash
   git clone https://github.com/votre-utilisateur/ohmyfood.git
   ```

2. Accédez au répertoire du projet :
   ```bash
   cd ohmyfood
   ```

3. Ouvrez `index.html` dans votre navigateur préféré pour voir le site en action.

## Utilisation

1. Accédez à la page d'accueil du site.
2. Sélectionnez un restaurant pour voir son menu.
3. Cliquez sur les cœurs pour ajouter des restaurants à vos favoris.
4. Utilisez le bouton "Commander" pour simuler une commande.

## Structure du projet

Voici la structure des fichiers et répertoires principaux du projet :

```
ohmyfood/
│
├── assets/
│   ├── css/
│   │   ├── style.css
│   │   ├── style-menu.css
│   ├── images/
│       ├── logo/
│       ├── restaurants/
│
├── index.html
├── restaurant.html
├── README.md
```

## Animations et choix techniques

### Animation du cœur

L'animation du cœur est réalisée en utilisant des pseudo-éléments CSS et des transitions. Voici un extrait de code CSS :

```css
.card-restaurant-rating-icone {
    cursor: pointer;
    transition: color 0.3s;
}

.card-restaurant-rating-icone-hover {
    display: none;
    color: var(--secondary-color);
}

.rating-checkbox:checked ~ .card-restaurant-rating-icone {
    display: none;
}

.rating-checkbox:checked ~ .card-restaurant-rating-icone-hover {
    display: inline-block;
}
```

### Sélecteur de plat

Le sélecteur de plat utilise des div et des classes pour styliser les éléments du menu. Chaque élément de menu change de style lors du survol pour indiquer qu'il est interactif.

### Choix des animations

- **Typing Animation** : Utilisée pour le titre principal avec une animation de frappe.
- **Fade-In Animation** : Utilisée pour afficher progressivement les sections de la page.
- **Slide-In Animation** : Utilisée pour afficher les éléments supplémentaires des cartes de menu lors du survol.

Exemple de l'animation de frappe :

```css
@keyframes typing {
    from {
        width: 0;
    }
    to {
        width: 100%;
    }
}
```

### Conception mobile first

Le projet est conçu avec une approche mobile first, en commençant par les styles pour les petits écrans puis en ajoutant des media queries pour les écrans plus larges.

```css
/* Styles par défaut pour les mobiles */
body {
    font-size: 16px;
    background-color: white;
    color: #353535;
}

/* Tablette */
@media (min-width: 768px) {
    .content {
        padding-top: 40px;
        padding-bottom: 50px;
        width: 80%;
    }
}

/* Desktop */
@media (min-width: 1024px) {
    .content {
        padding-top: 50px;
        padding-bottom: 60px;
        width: 70%;
    }
}


## Auteur

Claire GACHELIN
- GitHub: [Ma-Eum GitHub](https://github.com/Ma-Eum)
- OhMyFood: (https://ma-eum.github.io/Ohmyfood_Gachelin_Claire_3_code_052024/)
---

