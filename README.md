# ScoreCounter — Releases

Ce repo héberge les **binaires** et le **manifeste de mise à jour** de [ScoreCounter](https://github.com/kurokirito/score-counter), une app de comptage de scores pour jeux de société (Android + Windows).

Le code source est dans un repo privé. Ici on ne publie que les fichiers nécessaires à l'app pour se mettre à jour.

## Manifeste

L'app fetch [`update.json`](./update.json) au lancement pour détecter une nouvelle version :

```json
{
  "latest": "0.2.0",
  "buildCode": 261207,
  "publishedAt": "2026-12-07",
  "notes": "## Ajouts\n- ...",
  "platforms": {
    "android": { "url": "...apk", "sha256": "...", "size": 12345 },
    "windows": { "url": "...zip", "sha256": "...", "size": 67890 }
  }
}
```

## Téléchargements

Voir les [Releases GitHub](https://github.com/kurokirito/score-counter-releases/releases). Chaque release contient :

- `ScoreCounter-android-vX.Y.Z.apk` — APK signé pour installation directe (autoriser les sources inconnues)
- `ScoreCounter-win-x64-vX.Y.Z.zip` — bundle portable Windows à dézipper et lancer `ScoreCounter.exe`

## Installation manuelle

### Android
1. Télécharge l'APK depuis la dernière release
2. Autorise l'installation depuis l'application qui a téléchargé le fichier (Paramètres > Sécurité > Sources inconnues)
3. Ouvre l'APK et installe

### Windows
1. Télécharge le ZIP
2. Dézippe dans un dossier (ex. `C:\Apps\ScoreCounter`)
3. Lance `ScoreCounter.exe`
