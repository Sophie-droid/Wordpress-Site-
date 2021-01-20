# Wordpress-Site-

Création d'un site d'e-commerce avec WordPress

J'ai créer un site e-commerce de vente de bonbons.

Installation

Pour créer son site Wordpress en local, on installe  [LocalWP](https://localwp.com/). Ensuite, on se connecte à son compte Wordpress et on l'associe à un compte Flywheel.

Plugins installés

-   **WooCommerce**  : boîte à outil e-commerce
-   **WooCommerce AJAX Cart** : configuration des taxes, des étiquettes d'expédition et des paiements
-   **Elementor** :site responsive
-   **Yoast SEO**  : référencement
-   **WP Forms**  : création de formulaires (contact, newsletters,...)
-   **WPGlobus** : gestion multilingues
-   **GDPR Cookie Consent**  : gestion RGPD et cookies

Thème

On choisit un thème afin que l'on modifie

```
graph LR
A(Apparence) --> B(Thèmes)
B --> C(Télécharger thème)

```

Modification Menu
modifier le menu dans le tableau de bord

```
graph LR
A(Dashboard) --> B(Apparence)
B --> C(Menus)
C --> D(Compléter le formulaire)
C --> E(Ajouter les pages au menu)

```

Ajouter des catégories et des produits

Ajouter les catégories ainsi que les produits :
```
graph LR
A(Dashboard) --> B(Produits)
B --> C(Cathégorie)
B --> D(Ajouter)
C --> E(Compléter le formulaire)
D --> E

```

-   Dans la DataBase de Local (SQL) :

```
graph LR
A(select wp_wc_product_meta_lookup) -->B(Nouvel élément)
B --> C(Compléter le formulaire)

```

Créer des comptes clients et administrateurs

Créer des comptes clients :

```
graph LR
A(select wp_wc_customer_lookup) --> B(Nouvel élément)
B --> C(Compléter la fiche )


```
graph LR
A(Dashboard) --> B(Comptes)
B --> C(Ajouter)
C --> D(Compléter le formulaire)

```

-   Dans la DataBase de Local (SQL) :

```
graph LR
A(select wp_wc_product_meta_lookup) -->B(Nouvel élément)
B --> C(Compléter la fiche produit)
