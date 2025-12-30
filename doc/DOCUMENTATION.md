# EduSanté360 - Documentation Technique

## Table des Matières

1. [Présentation du Projet](#présentation-du-projet)
2. [Structure du Projet](#structure-du-projet)
3. [Technologies Utilisées](#technologies-utilisées)
4. [Architecture du Site](#architecture-du-site)
5. [Guide d'Installation](#guide-dinstallation)
6. [Guide d'Utilisation](#guide-dutilisation)
7. [Personnalisation](#personnalisation)
8. [Responsive Design](#responsive-design)
9. [Accessibilité](#accessibilité)
10. [Maintenance](#maintenance)
11. [Troubleshooting](#troubleshooting)

---

## Présentation du Projet

**EduSanté360** est un site web moderne et structuré dédié à l'éducation thérapeutique du patient diabétique. Il sert de guide complet pour les professionnels de santé et les patients.

### Objectifs

- Fournir un outil scientifique et pédagogique accessible
- Offrir un référentiel académique sur le diabète et l'ETP
- Harmoniser les pratiques éducatives
- Faciliter l'accès à l'information sur le diabète

### Public Cible

- Professionnels de santé (médecins, infirmiers, diététiciens, etc.)
- Étudiants en sciences de la santé
- Patients diabétiques et leurs proches
- Structures de soins

---

## Structure du Projet

```
EduSanté360/
│
├── index.html              # Page d'accueil
├── diabete.html            # Page sur les bases du diabète
├── etp.html                # Page sur l'éducation thérapeutique
├── ateliers.html           # Page des ateliers pratiques
├── ressources.html         # Page des ressources et annexes
├── contact.html            # Page de contact
│
├── css/
│   └── style.css           # Feuille de style principale
│
├── js/
│   └── script.js           # Scripts JavaScript
│
├── doc/
│   └── DOCUMENTATION.md    # Documentation technique
│
└── README.md               # Fichier README du projet
```

---

## Technologies Utilisées

### Frontend

- **HTML5** : Structure sémantique moderne
- **CSS3** : Styles et animations
  - Variables CSS personnalisées
  - Flexbox et Grid Layout
  - Animations et transitions
  - Media queries pour le responsive
- **JavaScript (ES6+)** : Interactivité
  - Navigation mobile
  - Animations au scroll
  - Gestion de formulaires
  - Notifications

### Bibliothèques Externes

- **Font Awesome 6.4.0** : Icônes
  - CDN : `https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css`

### Polices

- **Segoe UI** : Police principale
- **Arial** : Police pour les titres

---

## Architecture du Site

### Pages Principales

#### 1. Page d'Accueil (index.html)

**Sections :**
- Hero Section : Présentation visuelle avec appel à l'action
- Introduction : Contexte, objectifs et public cible
- Statistiques : Chiffres clés sur le diabète
- Topics : Navigation vers les sections principales
- CTA : Appel à l'action final

**Fonctionnalités :**
- Navigation sticky
- Animations au défilement
- Liens rapides vers les autres pages

#### 2. Page Diabète (diabete.html)

**Sections :**
- Définition du diabète
- Typologie (Type 1, Type 2, Gestationnel, Autres)
- Diagnostic biologique
- Complications (aiguës et chroniques)

**Éléments visuels :**
- Cartes colorées par type
- Tableaux de données
- Badges et alertes
- Grilles de complications

#### 3. Page ETP (etp.html)

**Sections :**
- Définition de l'ETP
- Objectifs (généraux et spécifiques)
- Pour qui et par qui
- Compétences du professionnel
- Démarche éducative structurée (4 étapes)
- Méthodes et outils pédagogiques

**Éléments visuels :**
- Timeline du processus
- Grilles de compétences
- Cartes d'information
- Citations encadrées

#### 4. Page Ateliers (ateliers.html)

**Sections :**
- Grille des 7 ateliers :
  1. Mieux connaître le diabète
  2. Autosurveillance glycémique
  3. Insulinothérapie
  4. Alimentation & activité physique
  5. Grossesse & diabète gestationnel
  6. Pied diabétique
  7. Diabète & Ramadan
- Détails approfondis des ateliers

**Fonctionnalités :**
- Navigation par ancre
- Cartes interactives
- Tableaux de valeurs cibles
- Guides étape par étape

#### 5. Page Ressources (ressources.html)

**Sections :**
- Grille de ressources disponibles
- Questionnaire d'évaluation complet
- Bibliographie indicative
- Section téléchargement

**Fonctionnalités :**
- Questionnaire interactif
- Listes organisées
- Boutons de téléchargement

#### 6. Page Contact (contact.html)

**Sections :**
- Informations de contact
- Formulaire de contact

**Fonctionnalités :**
- Validation de formulaire
- Notifications de succès/erreur
- Design responsive

---

## Guide d'Installation

### Prérequis

- Navigateur web moderne (Chrome, Firefox, Safari, Edge)
- Éditeur de code (VS Code, Sublime Text, etc.)
- Serveur web local (optionnel) : Live Server, XAMPP, etc.

### Installation Locale

1. **Cloner ou télécharger le projet**
   ```bash
   git clone [url-du-projet]
   cd EduSanté360
   ```

2. **Structure des dossiers**
   Assurez-vous que tous les dossiers sont présents :
   - `/css`
   - `/js`
   - `/doc`

3. **Ouvrir le site**
   
   **Option A : Directement dans le navigateur**
   ```
   Double-cliquez sur index.html
   ```
   
   **Option B : Avec un serveur local**
   ```bash
   # Avec Live Server (VS Code)
   Clic droit sur index.html > Open with Live Server
   
   # Avec Python
   python -m http.server 8000
   # Puis ouvrir http://localhost:8000
   ```

### Vérification

1. Ouvrez `index.html` dans votre navigateur
2. Vérifiez que :
   - Le header s'affiche correctement
   - Les styles sont appliqués
   - Les icônes Font Awesome s'affichent
   - La navigation fonctionne
   - Le menu mobile fonctionne sur petit écran

---

## Guide d'Utilisation

### Navigation

#### Menu Principal

Le menu de navigation est accessible en haut de chaque page :
- **Accueil** : Retour à la page d'accueil
- **Le Diabète** : Informations scientifiques
- **ETP** : Éducation thérapeutique
- **Ateliers** : Ateliers pratiques
- **Ressources** : Documents et annexes
- **Contact** : Formulaire de contact

#### Navigation Mobile

Sur mobile (< 768px) :
1. Cliquez sur le bouton hamburger (☰)
2. Le menu s'ouvre en overlay
3. Cliquez sur un lien pour naviguer
4. Le menu se ferme automatiquement

### Fonctionnalités Interactives

#### Bouton Scroll to Top

- Apparaît après avoir scrollé 300px
- Clic pour retour en haut de page
- Animation smooth

#### Animations au Scroll

- Les cartes apparaissent avec une animation fade-in
- Activées par Intersection Observer
- Performances optimisées

#### Formulaire de Contact

1. Remplir tous les champs obligatoires (*)
2. Sélectionner un sujet
3. Cliquer sur "Envoyer le message"
4. Une notification confirme l'envoi

**Validation :**
- Email valide requis
- Champs obligatoires vérifiés
- Messages d'erreur affichés si nécessaire

---

## Personnalisation

### Couleurs

Les couleurs sont définies dans `:root` dans `style.css` :

```css
:root {
    --primary-color: #2563eb;      /* Bleu principal */
    --secondary-color: #10b981;    /* Vert secondaire */
    --accent-color: #f59e0b;       /* Orange accent */
    --danger-color: #ef4444;       /* Rouge danger */
    --dark-color: #1e293b;         /* Texte foncé */
    --light-color: #f8fafc;        /* Fond clair */
    --gray-color: #64748b;         /* Gris texte */
    --white: #ffffff;              /* Blanc */
}
```

**Pour changer les couleurs :**
1. Ouvrez `css/style.css`
2. Modifiez les valeurs dans `:root`
3. Sauvegardez et rechargez la page

### Typographie

**Polices actuelles :**
```css
--font-primary: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
--font-heading: 'Arial', sans-serif;
```

**Pour changer les polices :**
1. Ajoutez un lien Google Fonts dans le `<head>` si nécessaire
2. Modifiez les variables dans `:root`
3. Exemple :
   ```html
   <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
   ```
   ```css
   --font-primary: 'Roboto', sans-serif;
   ```

### Logo

**Pour ajouter un logo personnalisé :**
1. Remplacez l'icône Font Awesome dans `.logo` :
   ```html
   <!-- Ancien -->
   <div class="logo">
       <i class="fas fa-heartbeat"></i>
       <span>EduSanté360</span>
   </div>
   
   <!-- Nouveau -->
   <div class="logo">
       <img src="img/logo.png" alt="Logo">
       <span>EduSanté360</span>
   </div>
   ```

2. Ajoutez le CSS pour l'image :
   ```css
   .logo img {
       height: 40px;
       width: auto;
   }
   ```

### Hero Section

**Pour changer l'image de fond :**
```css
.hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    /* Remplacez par : */
    background: url('../img/hero-bg.jpg') center/cover no-repeat;
}
```

---

## Responsive Design

### Breakpoints

Le site utilise 3 breakpoints principaux :

```css
/* Desktop : > 992px (défaut) */

/* Tablette : 768px - 992px */
@media (max-width: 992px) { }

/* Mobile : < 768px */
@media (max-width: 768px) { }
```

### Adaptations Mobile

#### Navigation
- Menu hamburger activé
- Menu overlay plein écran
- Fermeture automatique au clic

#### Grilles
- Passage en colonne unique
- Cards empilées verticalement

#### Typographie
- Tailles de titres réduites
- Espacement adapté

#### Hero
- Hauteur réduite à 500px
- Boutons empilés verticalement

### Tests Responsive

**Tester le design responsive :**
1. Ouvrez les DevTools (F12)
2. Activez le mode responsive (Ctrl+Shift+M)
3. Testez les différentes résolutions :
   - Mobile : 375px, 414px
   - Tablette : 768px, 1024px
   - Desktop : 1280px, 1920px

---

## Accessibilité

### Principes Appliqués

#### Sémantique HTML
- Utilisation correcte des balises sémantiques
- `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`
- Hiérarchie des titres respectée (h1 → h6)

#### ARIA
- `aria-label` sur les boutons sans texte
- `role` sur les éléments interactifs si nécessaire

#### Navigation Clavier
- Tous les liens et boutons sont accessibles au clavier
- `Tab` pour naviguer
- `Enter` pour activer

#### Contraste
- Ratios de contraste respectés (WCAG AA)
- Texte lisible sur tous les fonds

#### Focus Visible
- Outline visible sur les éléments focusés
- Styles de focus personnalisés

### Améliorations Possibles

1. **Ajout de skip links**
   ```html
   <a href="#main-content" class="skip-link">Aller au contenu principal</a>
   ```

2. **ARIA landmarks**
   ```html
   <nav role="navigation" aria-label="Navigation principale">
   ```

3. **Alt text pour images futures**
   ```html
   <img src="..." alt="Description précise">
   ```

---

## Maintenance

### Mise à Jour du Contenu

#### Modifier le Texte

1. Ouvrez le fichier HTML concerné
2. Localisez la section à modifier
3. Éditez le texte directement dans le HTML
4. Sauvegardez et testez

#### Ajouter une Nouvelle Section

```html
<section class="section">
    <div class="container">
        <div class="section-header">
            <h2>Nouveau Titre</h2>
            <div class="divider"></div>
        </div>
        <div class="content-grid">
            <!-- Votre contenu -->
        </div>
    </div>
</section>
```

#### Ajouter un Nouvel Atelier

1. Ajoutez une carte dans `.workshops-grid` :
   ```html
   <div class="workshop-card">
       <div class="workshop-icon nouveau-type">
           <i class="fas fa-icon-name"></i>
       </div>
       <h3>Titre Atelier</h3>
       <p>Description</p>
       <ul class="workshop-topics">
           <li><i class="fas fa-check"></i> Point 1</li>
       </ul>
       <a href="#atelier-id" class="btn btn-outline">En savoir plus</a>
   </div>
   ```

2. Ajoutez le style pour l'icône :
   ```css
   .workshop-icon.nouveau-type {
       background: linear-gradient(135deg, #couleur1, #couleur2);
   }
   ```

3. Ajoutez la section détaillée avec l'id correspondant

### Mise à Jour des Styles

#### Modifier un Style Existant

1. Ouvrez `css/style.css`
2. Utilisez la recherche (Ctrl+F) pour trouver la classe
3. Modifiez les propriétés CSS
4. Testez dans le navigateur

#### Ajouter un Nouveau Style

```css
/* Ajoutez à la fin de style.css ou dans la section appropriée */
.nouvelle-classe {
    propriété: valeur;
}
```

### Sauvegarde

**Recommandations :**
1. Utilisez un système de contrôle de version (Git)
2. Sauvegardez régulièrement
3. Testez avant de déployer en production
4. Gardez une copie de backup

---

## Troubleshooting

### Problèmes Courants

#### Les Styles ne s'Appliquent Pas

**Solutions :**
1. Vérifiez le chemin du fichier CSS :
   ```html
   <link rel="stylesheet" href="css/style.css">
   ```
2. Videz le cache du navigateur (Ctrl+Shift+R)
3. Vérifiez la console pour des erreurs (F12)
4. Assurez-vous qu'il n'y a pas d'erreur de syntaxe CSS

#### Les Icônes Font Awesome ne s'Affichent Pas

**Solutions :**
1. Vérifiez la connexion Internet
2. Vérifiez le lien CDN :
   ```html
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
   ```
3. Vérifiez les classes d'icônes :
   ```html
   <i class="fas fa-heart"></i>
   ```

#### Le Menu Mobile ne Fonctionne Pas

**Solutions :**
1. Vérifiez que script.js est bien chargé :
   ```html
   <script src="js/script.js"></script>
   ```
2. Ouvrez la console (F12) pour voir les erreurs JavaScript
3. Vérifiez que les classes CSS correspondent :
   - `.nav-toggle`
   - `.nav-menu`

#### Les Animations ne Fonctionnent Pas

**Solutions :**
1. Vérifiez que JavaScript est activé dans le navigateur
2. Testez dans un autre navigateur
3. Vérifiez la console pour des erreurs

#### Le Formulaire ne s'Envoie Pas

**Solutions :**
1. C'est normal - le formulaire simule un envoi
2. Pour un vrai envoi, ajoutez un backend :
   ```javascript
   // Dans script.js
   fetch('/api/contact', {
       method: 'POST',
       body: JSON.stringify(formData),
       headers: { 'Content-Type': 'application/json' }
   })
   ```

### Performance

#### Site Lent à Charger

**Optimisations :**
1. Minifiez CSS et JS
2. Optimisez les images (compression)
3. Utilisez un CDN pour les librairies
4. Activez la mise en cache

#### Animations Saccadées

**Solutions :**
1. Utilisez `transform` et `opacity` pour les animations
2. Évitez d'animer `width`, `height`, `top`, `left`
3. Utilisez `will-change` avec parcimonie
4. Testez sur différents appareils

---

## Déploiement

### Hébergement Web

#### Options d'Hébergement

1. **GitHub Pages** (Gratuit)
   - Parfait pour les sites statiques
   - Configuration facile
   - URL : `username.github.io/edusante360`

2. **Netlify** (Gratuit)
   - Déploiement automatique depuis Git
   - HTTPS inclus
   - Domaine personnalisé

3. **Vercel** (Gratuit)
   - Excellent pour les sites statiques
   - Déploiement rapide

4. **Hébergement traditionnel**
   - OVH, Hostinger, etc.
   - Nécessite FTP

#### Déploiement sur GitHub Pages

```bash
# 1. Créer un repo sur GitHub
# 2. Push le code
git init
git add .
git commit -m "Initial commit"
git remote add origin [url-du-repo]
git push -u origin main

# 3. Activer GitHub Pages
# Settings > Pages > Source: main branch
```

### Domaine Personnalisé

1. Achetez un nom de domaine
2. Configurez les DNS :
   ```
   Type: A
   Host: @
   Value: [IP du serveur]
   ```
3. Ajoutez le domaine dans les paramètres d'hébergement

---

## Évolutions Futures

### Fonctionnalités à Ajouter

1. **Système de Recherche**
   - Barre de recherche globale
   - Filtrage des ateliers

2. **Multilingue**
   - Français / Arabe
   - Sélecteur de langue

3. **Mode Sombre**
   - Toggle dark/light mode
   - Préférence sauvegardée

4. **Backend**
   - API pour le formulaire
   - Base de données des patients
   - Système d'authentification

5. **PWA (Progressive Web App)**
   - Fonctionnement offline
   - Installation sur mobile

6. **PDF Générables**
   - Générer des fiches PDF
   - Téléchargement des ressources

---

## Support et Contact

Pour toute question ou problème technique :

- **Email** : info@edusante360.dz
- **Documentation** : Voir ce fichier
- **Issues** : Si le projet est sur GitHub

---

## Crédits

- **Développement** : EduSanté360 Team
- **Contenu** : Basé sur les recommandations de l'OMS, HAS, ADA, IDF
- **Icônes** : Font Awesome
- **Polices** : Système (Segoe UI, Arial)

---

## License

Ce projet est destiné à un usage éducatif et médical. Tous droits réservés © 2025 EduSanté360.

---

**Version de la Documentation** : 1.0  
**Dernière Mise à Jour** : Décembre 2025  
**Auteur** : EduSanté360 Development Team


