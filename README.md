# Jean Store - E-Commerce Premium

Une application e-commerce moderne et complète dédiée à la vente de jeans de haute qualité. Disponible en version **Web** et **Mobile App**.

## 🎯 Caractéristiques

- ✅ Design premium minimaliste (Noir, Blanc, Gris, Bleu nuit)
- ✅ Responsive (Mobile, Tablet, Desktop)
- ✅ Interface type application mobile (PWA ready)
- ✅ Panier dynamique et checkout fluide
- ✅ Système de paiement multi-options (Stripe, PayPal, Orange Money, Livraison)
- ✅ Compte utilisateur avec historique
- ✅ Admin panel sécurisé (propriétaire uniquement)
- ✅ Bilingue (Français/Anglais)
- ✅ Chat WhatsApp intégré
- ✅ Adapté au marché guinéen

## 📱 Versions

### Web Version
- Accessible via navigateur
- Tous les appareils (Mobile, Tablet, PC)
- PWA (Progressive Web App)
- URL: `https://jean-store.vercel.app`

### Mobile App Version
- Native-like experience
- Optimisée pour iOS et Android
- Installation directe sur l'appareil

## 🛠️ Tech Stack

### Frontend
- HTML5
- CSS3 (Animations, Flexbox, Grid)
- JavaScript (Vanilla + Axios)
- React (version mobile app)

### Backend
- Node.js
- Express.js
- MongoDB
- JWT pour authentification

### Paiements
- Stripe (Carte bancaire)
- PayPal API
- Orange Money API
- Paiement à la livraison

### Hébergement
- Frontend: Vercel
- Backend: Render
- DB: MongoDB Atlas

## 📁 Structure du Projet

```
jean-store/
├── web/                          # Version Web Site
│   ├── index.html               # Accueil
│   ├── products.html            # Catalogue produits
│   ├── product-detail.html      # Détail produit
│   ├── cart.html                # Panier
│   ├── checkout.html            # Paiement/Commande
│   ├── account.html             # Profil utilisateur
│   ├── admin.html               # Panel admin (sécurisé)
│   ├── css/
│   │   ├── style.css            # Styles principaux
│   │   ├── responsive.css       # Styles responsive
│   │   └── animations.css       # Animations
│   ├── js/
│   │   ├── app.js               # Logique principale
│   │   ├── api.js               # Appels API
│   │   ├── cart.js              # Gestion panier
│   │   ├── auth.js              # Authentification
│   │   └── admin.js             # Fonctions admin
│   └── assets/
│       ├── logo.svg
│       └── images/
│
├── mobile/                       # Version App Mobile
│   ├── package.json
│   ├── index.html
│   ├── manifest.json            # PWA Manifest
│   ├── css/
│   │   ├── app.css              # Styles mobiles
│   │   └── animations.css
│   ├── js/
│   │   ├── app.js
│   │   ├── screens.js
│   │   └── api.js
│   └── assets/
│
├── backend/                      # Serveur Backend
│   ├── server.js                # Point d'entrée
│   ├── package.json
│   ├── .env.example
│   ├── config/
│   │   ├── db.js                # MongoDB connection
│   │   └── env.js               # Variables d'environnement
│   ├── routes/
│   │   ├── products.js          # CRUD produits
│   │   ├── orders.js            # Gestion commandes
│   │   ├── users.js             # Gestion utilisateurs
│   │   ├── auth.js              # Authentification
│   │   ├── admin.js             # Routes admin
│   │   └── payments.js          # Paiements
│   ├── models/
│   │   ├── User.js              # Schéma utilisateur
│   │   ├── Product.js           # Schéma produit
│   │   ├── Order.js             # Schéma commande
│   │   └── Cart.js              # Schéma panier
│   ├── controllers/
│   │   ├── productController.js
│   │   ├── orderController.js
│   │   ├── userController.js
│   │   └── adminController.js
│   ├── middleware/
│   │   ├── auth.js              # Auth middleware
│   │   └── adminAuth.js         # Admin auth middleware
│   ├── utils/
│   │   ├── payment.js           # Intégrations paiements
│   │   ├── email.js             # Service email
│   │   └── logger.js            # Logging
│   └── uploads/                 # Images produits
│
├── public/
│   ├── favicon.ico
│   └── robots.txt
│
└── .gitignore
```

## 🚀 Installation et Démarrage

### Backend
```bash
cd backend
npm install
cp .env.example .env
# Configurez vos variables d'environnement
npm start
```

### Frontend Web
```bash
# Ouvrir simplement dans le navigateur
open web/index.html
# Ou en local server:
cd web
python -m http.server 8000
# ou avec Node:
npx http-server
```

### Frontend Mobile
```bash
cd mobile
npm install
npm start
```

## 🔐 Admin Panel

**Accès**: `/admin.html` ou `/admin`
**Authentification**: Email propriétaire + Mot de passe sécurisé (JWT)
**Fonctionnalités**:
- ➕ Ajouter/Modifier/Supprimer produits
- 📊 Tableau de bord avec KPIs
- 📦 Gestion des commandes
- 💬 Chat client (WhatsApp intégré)
- 📈 Statistiques de ventes
- 👥 Gestion utilisateurs
- 💰 Suivi des revenus

⚠️ **Important**: Seul le propriétaire (celso2k8) peut accéder à l'admin panel. Les visiteurs ne peuvent que consulter et acheter.

## 💳 Paiements Supportés

- 💳 **Carte bancaire** (Stripe)
- 🔵 **PayPal**
- 🟠 **Orange Money**
- 🚚 **Paiement à la livraison**

## 🌍 Localisation

- 🇫🇷 Français
- 🇬🇧 Anglais
- 🇬🇳 **Guinée**: Livraison Conakry + villes, numéros +224, support WhatsApp

## 📧 Contact Client

- **WhatsApp**: +224 xxx xxx xxx (Boutton intégré)
- **Email**: contact@jeanstore.gy
- **Localisation**: Conakry, Guinée 🇬🇳

## 📊 Environnements

### Développement
- Backend: `http://localhost:5000`
- Frontend Web: `http://localhost:8000`
- Frontend Mobile: `http://localhost:3000`

### Production
- Backend: Render
- Frontend: Vercel
- DB: MongoDB Atlas

## 📝 Variables d'Environnement

Voir `.env.example` dans le dossier `backend`

## 🤝 Contributeurs

- **Propriétaire**: celso2k8
- **Contact**: Via WhatsApp ou email

## 📄 Licence

Propriétaire exclusif: Jean Store

---

**Jean Store** - Premium Denim Collection
*Depuis Conakry, Guinée 🇬🇳*