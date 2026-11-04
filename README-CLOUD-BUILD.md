# STY Player — compilation APK dans le cloud

Ce projet est préparé pour être compilé par GitHub Actions, sans installer Android Studio sur le téléphone.

## Étapes depuis un téléphone Android

1. Créer ou ouvrir un compte GitHub.
2. Télécharger et extraire `STY_Player_Cloud_Build.zip` sur le téléphone.
3. Sur GitHub, créer un nouveau dépôt nommé `sty-player-android`.
4. Dans le dépôt, choisir **Add file → Upload files** et téléverser le contenu extrait du dossier du projet,
   y compris le dossier caché `.github/workflows` et son fichier `android-apk.yml`.
5. Valider avec **Commit changes** sur la branche `main`.
6. Ouvrir l'onglet **Actions** du dépôt. Le workflow **Build STY Player APK** doit démarrer.
7. Quand l'exécution est terminée avec une coche verte, ouvrir l'exécution et descendre à **Artifacts**.
   Télécharger `STY-Player-debug-APK`.
8. Extraire l'archive téléchargée : elle contient `app-debug.apk`. Ouvrir ce fichier pour installer l'application.

## Important — état réel du logiciel

- Le projet contient une interface sombre et les commandes de sections.
- Il contient un parseur MIDI Yamaha expérimental et l'intégration déclarée de FluidSynth.
- Il ne contient pas encore MuldjordKit.sf2 : l'écran permet de charger une SoundFont SF2 séparément.
- Les curseurs d'égaliseur sont encore désactivés.
- Les styles Yamaha varient selon les modèles PSR. Le parseur doit être testé avec de vrais fichiers STY avant de garantir leur compatibilité.
- L'APK généré est une version de test (debug), pas une version publiée sur Play Store.

Ne partage jamais ton mot de passe GitHub ni de code de connexion dans cette conversation.
