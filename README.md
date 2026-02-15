# Nozélis Landing Page

Landing page ultra moderne et sophistiquée pour le système financier TherapeuteFinances INAMI.

## 🎨 Design Features

- **Dark theme premium** avec accents néon (vert/violet)
- **Typographie distinctive** : Archivo (display) + JetBrains Mono (code)
- **Animations fluides** : fade-in, slide-up, pulse, rotate
- **Bento Grid Layout** pour les fonctionnalités
- **Navigation flottante** avec backdrop blur
- **Code preview animé** pour montrer la complexité du système
- **Responsive** : mobile-first design

## 🚀 Déploiement sur Vercel

### Option 1 : Déploiement via GitHub (Recommandé)

1. **Créer un repo GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Nozélis landing page"
   git branch -M main
   git remote add origin https://github.com/VOTRE_USERNAME/nozelis-landing.git
   git push -u origin main
   ```

2. **Connecter à Vercel**
   - Allez sur [vercel.com](https://vercel.com)
   - Cliquez sur "New Project"
   - Importez votre repo GitHub
   - Vercel détectera automatiquement que c'est un site statique
   - Cliquez sur "Deploy"

3. **Configuration**
   - Root Directory: `./`
   - Build Command: (laisser vide pour HTML statique)
   - Output Directory: `./`

### Option 2 : Déploiement via Vercel CLI

1. **Installer Vercel CLI**
   ```bash
   npm i -g vercel
   ```

2. **Déployer**
   ```bash
   cd /chemin/vers/votre/projet
   vercel
   ```

3. **Suivre les instructions**
   - Login avec votre compte Vercel
   - Confirmer les settings
   - Le site sera déployé automatiquement

### Option 3 : Drag & Drop (Le plus simple)

1. Allez sur [vercel.com/new](https://vercel.com/new)
2. Faites glisser le dossier contenant `index.html`
3. Vercel déploiera automatiquement

## 📝 Personnalisation

### Modifier les couleurs

Dans la section `:root` du CSS (lignes 17-27) :

```css
--midnight: #0A0E1A;      /* Fond principal */
--accent: #00F5A0;        /* Vert néon */
--purple: #A78BFA;        /* Violet */
--blue: #60A5FA;          /* Bleu */
```

### Modifier les textes

1. **Hero section** : lignes 226-280
2. **Features** : lignes 345-450
3. **Pricing** : lignes 550-620
4. **FAQ** : lignes 655-750

### Ajouter votre lien de paiement

Remplacez `VOTRE_LIEN_SYSTEME_IO` à la ligne 585 :

```html
<a href="https://votre-lien-systeme-io.com" class="btn btn-primary pricing-cta">
```

### Ajouter des screenshots réels

Remplacez les mockups dans :
- Hero visual (ligne 290)
- System preview (ligne 490)

Recommandations :
- Format : PNG avec fond transparent
- Taille : min 1200px de largeur
- Optimisez avec [TinyPNG](https://tinypng.com)

## 🎯 Optimisations

### Performance

1. **Fonts** : déjà optimisées avec `font-display: swap`
2. **Animations** : CSS-only pour performance maximale
3. **Images** : utilisez WebP pour réduire la taille

### SEO

Ajoutez dans le `<head>` :

```html
<meta name="description" content="Système financier intelligent pour thérapeutes INAMI. 14 onglets automatisés, calculs en temps réel.">
<meta name="keywords" content="INAMI, thérapeute, finances, Belgique, comptabilité">
<meta property="og:title" content="Nozélis - Système Financier INAMI">
<meta property="og:description" content="Le CFO dans votre feuille de calcul">
<meta property="og:image" content="https://votre-domaine.com/og-image.jpg">
```

### Analytics

Ajoutez avant le `</head>` :

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🔧 Structure du projet

```
nozelis-landing/
├── index.html          # Page principale (tout-en-un)
├── README.md          # Ce fichier
└── .gitignore         # (optionnel)
```

## 🌐 Domaine personnalisé

1. Sur Vercel, allez dans Settings > Domains
2. Ajoutez votre domaine
3. Suivez les instructions DNS fournies
4. Attendez la propagation (quelques heures max)

## 📱 Test responsive

Testez sur :
- Desktop : 1920px, 1440px, 1024px
- Tablet : 768px, 834px
- Mobile : 375px, 414px

Chrome DevTools > Toggle Device Toolbar (Cmd+Shift+M)

## 🎨 Inspirations design

Cette landing page utilise :
- Dark theme moderne (type Stripe, Linear)
- Glassmorphism (backdrop blur)
- Néon accents (type Vercel, Next.js)
- Typographie monospace pour l'aspect "technique"
- Bento grid (type Apple)

## 📞 Support

Pour toute question :
- Email : support@nozelis.com
- Documentation : docs.nozelis.com

## 📄 Licence

© 2025 Nozélis. Tous droits réservés.
