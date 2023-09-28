# Face Mask detection using YOLOv8
# KI-Gesichtsmaskenerkennung

<p align="center">
  <img src="./sample.png" />
</p>

**LINK zur KI-Gesichtsmaskenerkennung direkt in Browser:**
  https://miaoima.github.io/FaceMaskDetection/
---

**Model**

Verwendetes Modell ist das in tensorflow.js konvertierte YOLOv8n_FaceMask Modell.

Durch das Modell kann erkannt werden, ob Personen auf Bildern oder in Videos eine Maske tragen und ob die Maske korrekt getragen wird. Zudem kann die entsprechende Anzahl erfasst werden.

**Projekt auf GitHub Pages veröffentlichen**

### 1. Erstelle ein GitHub Repository
Falls du noch kein GitHub Repository erstellt hast, erstelle ein neues öffentliches Repository. Erstelle auf GitHub ein neues Repository und pushe dein lokales Projekt in dieses Repository.

### 2. Projektvorbereitung
Stelle sicher, dass dein Projekt bereits als Git Repository initialisiert ist und alle Änderungen committed wurden.

```sh
git init
git add .
git commit -m "Erstes Commit"
```

### 3. Pushe das Projekt auf GitHub
Verbinde dein lokales Repository mit dem GitHub Repository und pushe den Code auf GitHub.

```sh
git remote add origin https://github.com/Benutzername/Repositoryname.git
git push -u origin main
```

### 4. Installiere das `gh-pages` Paket
`gh-pages` ist ein Paket, dass den Prozess der Veröffentlichung auf GitHub Pages vereinfacht. Installiere es in deinem Projektverzeichnis mit dem folgenden Befehl:

```sh
yarn add gh-pages
```

### 5. Konfiguriere `package.json`
Füge in deiner `package.json` Datei ein `homepage` Feld und ein `deploy` Skript hinzu. Zum Beispiel:

```json
{
  "name": "Projektname",
  "homepage": "https://Benutzername.github.io/Repositoryname",
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "deploy": "yarn run build && gh-pages -d build",
    // ... andere Skripte
  },
  // ... andere Konfigurationen
}
```

### 6. Deploye das Projekt
Führe den folgenden Befehl aus, um dein Projekt zu bauen und auf GitHub Pages zu veröffentlichen:

```sh
yarn run deploy
```

### 7. Konfiguriere das GitHub Repository
Zuletzt, gehe zur Einstellungsseite deines GitHub Repositories, finde den GitHub Pages Bereich, und stelle sicher, dass der `gh-pages` Branch als Quell-Branch ausgewählt ist.

### 8. Besuche deine Webseite
Nun solltest du in der Lage sein, deine Webseite unter `https://Benutzername.github.io/Repositoryname` zu erreichen.

Denke daran, nach jeder Änderung am Projektcode `yarn run deploy` erneut auszuführen, um den Inhalt auf GitHub Pages zu aktualisieren.

### Formatierung für GitHub README:
```markdown
## Wie man ein Projekt auf GitHub Pages veröffentlicht

1. **[GitHub Repository erstellen](#1-erstelle-ein-github-repository)**
2. **[Projektvorbereitung](#2-projektvorbereitung)**
3. **[Pushe das Projekt auf GitHub](#3-pushe-das-projekt-auf-github)**
4. **[Installiere das gh-pages Paket](#4-installiere-das-gh-pages-paket)**
5. **[Konfiguriere package.json](#5-konfiguriere-packagejson)**
6. **[Deploye das Projekt](#6-deploye-das-projekt)**
7. **[Konfiguriere das GitHub Repository](#7-konfiguriere-das-github-repository)**
8. **[Besuche deine Webseite](#8-besuche-deine-webseite)**
```
## Reference

- https://github.com/ultralytics/ultralytics
- https://github.com/Hyuto/yolov8-onnxruntime-web
