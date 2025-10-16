🚀 Signalist : Stock Tracker
Suivez les prix des actions en temps réel.

🏁 Démarrage Rapide
Ce guide vous explique comment configurer et lancer le projet Signalist sur votre machine locale.

Prérequis
Assurez-vous que les outils suivants sont installés avant de commencer :

Git

Node.js (recommandé : LTS)

npm (gestionnaire de paquets Node)

1. Clonage du Dépôt
Ouvrez votre terminal et exécutez les commandes suivantes pour télécharger et accéder au dossier du projet :

Bash

git clone https://github.com/RiahiZaid/Signalist-Stock-Tracker
cd Signalist-Stock-Tracker-App
2. Installation des Dépendances
Installez toutes les bibliothèques et paquets nécessaires au fonctionnement du projet :

Bash

npm install
3. Configuration des Variables d'Environnement
Le projet nécessite plusieurs clés API et informations de connexion pour fonctionner.

Créez un nouveau fichier nommé .env à la racine de votre projet.

Copiez-y le contenu suivant et remplacez les valeurs de substitution (=) par vos propres identifiants.

مقتطف الرمز

NODE_ENV='development'
NEXT_PUBLIC_BASE_URL=http://localhost:3000

# FINNHUB (Données boursières en temps réel)
NEXT_PUBLIC_NEXT_PUBLIC_FINNHUB_API_KEY=
FINNHUB_BASE_URL=https://finnhub.io/api/v1

# MONGODB (Base de données)
MONGODB_URI=

# AUTHENTIFICATION (Better Auth)
BETTER_AUTH_SECRET=
BETTER_AUTH_URL=http://localhost:3000

# GEMINI (IA pour le traitement ou l'analyse)
GEMINI_API_KEY=

# NODEMAILER (Envoi d'e-mails, par exemple pour les alertes)
NODEMAILER_EMAIL=
NODEMAILER_PASSWORD=
⚠️ IMPORTANT : Vous devrez vous inscrire auprès des services suivants pour obtenir les clés nécessaires : Finnhub, MongoDB et Gemini.

4. Lancement du Projet
Pour lancer l'application, vous devez démarrer le serveur Next.js et l'outil de développement Inngest (pour les fonctions asynchrones/tâches planifiées).

Démarrez le serveur Next.js en mode développement :

Bash

npm run dev
Dans un second terminal, démarrez l'outil de développement Inngest :

Bash

npx inngest-cli@latest dev
5. Accès à l'Application
Une fois les deux serveurs lancés, ouvrez votre navigateur et accédez à :

👉 http://localhost:3000
