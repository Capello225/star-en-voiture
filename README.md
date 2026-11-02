# 🚗 Star en Voiture

Ta photo prend vie devant une voiture de luxe : l'IA **Agnes** crée des vidéos verticales (9:16) où la personne de la photo
marche devant la voiture que tu décris et prononce ton texte.

## 📲 Installer

| Téléphone | Comment |
|---|---|
| **Android** | Télécharge **[Star-en-Voiture.apk](https://github.com/Capello225/star-en-voiture/releases/latest/download/Star-en-Voiture.apk)**, ouvre le fichier et autorise l'installation. |
| **iPhone** | Ouvre **[capello225.github.io/star-en-voiture](https://capello225.github.io/star-en-voiture/)** dans **Safari** → bouton **Partager** → **« Sur l'écran d'accueil »**. |
| Ordinateur | Même lien que l'iPhone, dans n'importe quel navigateur. |

## 🔑 Clé API (gratuite)

1. Va sur [platform.agnes-ai.com](https://platform.agnes-ai.com) → **API Keys** → **Create new secret key**.
2. Colle la clé dans l'application → **Enregistrer la clé**.

La clé reste uniquement sur ton téléphone : elle n'est jamais dans le code ni envoyée ailleurs qu'à Agnes.

## ✨ Fonctions

- 1 photo → jusqu'à 10 vidéos différentes (caméra, lumière, mouvement aléatoires) · plusieurs photos → 1 vidéo par photo
- Voiture, texte prononcé et scène personnalisables · durée de 3 à 10 s
- File d'attente automatique (1 vidéo / minute, limite du compte gratuit Agnes), ralentit seule si l'API le demande
- Écran maintenu allumé, reprise des vidéos en cours après fermeture
- Enregistrement dans la galerie / partage direct (WhatsApp, TikTok…)

## ⚠️ Bon à savoir

- Compte gratuit Agnes : environ 1 vidéo par minute ; les limites peuvent changer.
- Le texte prononcé et le mouvement des lèvres sont approximatifs avec le modèle gratuit : préfère des phrases courtes.
- Utilise uniquement des photos de toi ou de personnes qui ont donné leur accord.

## 🛠️ Technique

- `www/index.html` : l'application complète (un seul fichier), aussi utilisée par l'APK.
- `android/` : projet Capacitor 8.
- `.github/workflows/build.yml` : à chaque envoi sur `main`, compile l'APK signé (Releases) et publie la version web (GitHub Pages).
