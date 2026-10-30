# Aplomb

[Télécharger l’APK](https://github.com/Zachiran42/aplomb/releases/latest/download/aplomb-0.1.0.apk) · [Versions](https://github.com/Zachiran42/aplomb/releases) · [Page du jeu](https://zachiran42.github.io/aplomb/)

Prototype Android natif, hors ligne, sans permission ni publicité. Android 8+. Partie courte, record local, pause et reprise.

Huit pièces : glisser horizontalement puis relâcher. Le centre de masse doit rester sur chaque support. Déborder rapporte davantage.

Sources Java et Canvas, licence MIT. Le script scripts/build.ps1 prend un fichier toolchain et une clé externe ; ne jamais publier de clé. APK de développement, pas encore testé sur téléphone physique.

## Dans Cercle

Dans « Ajouter depuis GitHub », coller `https://github.com/Zachiran42/aplomb`. La dernière Release contient un seul APK, signé, universel et sans permission Internet.

## Compilation

Copier `.toolchain.example.json` vers `.toolchain.json`, renseigner JDK21, Android SDK36 et Build Tools, puis définir `MINIGAMES_KEYSTORE_PASSWORD` dans l’environnement. Utiliser `scripts/build.ps1 -KeyStore C:/cles/jeu.keystore -KeyAlias votre-alias`. Garder les clés hors du dépôt.
