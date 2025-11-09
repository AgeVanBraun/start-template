# 🧠 Git + GitHub Cheatsheet für meine Projekte

## 🚀 Projekt starten

```bash
mkdir meinProjekt
cd meinProjekt
git init
```

---

## 📄 Dateien erstellen

(z. B. index.html, style.css, script.js)

---

## ✅ Änderungen speichern

```bash
git add .
git commit -m "Erster Stand des Projekts"
```

---

## ☁️ GitHub-Repo erstellen

1. Gehe zu https://github.com
2. Klicke auf **„+“ → „New repository“**
3. Name z. B. `meinProjekt` eingeben
4. Kein README anlegen
5. Auf **„Create repository“** klicken

---

## 🔗 GitHub verknüpfen

```bash
git remote add origin https://github.com/DEINNAME/meinProjekt.git
```

_(`DEINNAME` & `meinProjekt` anpassen)_

---

## 🧭 Branch prüfen

```bash
git branch
```

- Wenn `main`:

```bash
git push -u origin main
```

- Wenn `master`:

```bash
git push -u origin master
```

---

## 🔁 Spätere Änderungen hochladen

```bash
git add .
git commit -m "Neuer Stand"
git push
```

---

## 🧾 Kurz-Erklärungen

| Befehl             | Bedeutung                       |
| ------------------ | ------------------------------- |
| `git init`         | Git starten                     |
| `git add .`        | alle Änderungen vormerken       |
| `git commit -m ""` | Änderung benennen und speichern |
| `git push`         | Hochladen zu GitHub             |
| `git branch`       | zeigt aktuellen Branch          |
| `git remote add`   | Verbindung zu GitHub herstellen |

---

# 🧠 GitHub Workflow – Neues Projekt aus Template erstellen

Dieser Ablauf zeigt, wie du ein bestehendes Template von GitHub lokal klonst, anpasst und daraus ein neues Repository auf GitHub erstellst.

---

## ⚙️ 1. Lokalen Projektordner anlegen

mkdir myNewProject
cd myNewProject

---

## 📥 2. Template klonen

```bash
git clone https://github.com/AgeVanBraun/start-template.git .
```

**Hinweis:**
Der Punkt `.` am Ende bedeutet, dass alle Dateien direkt in den aktuellen Ordner (`myNewProject`) kopiert werden.

---

## 🧹 3. Alte Remote-Verbindung löschen

Nach dem Klonen zeigt `git remote -v` noch auf das alte Template.
Diese Verbindung entfernst du:

```bash
git remote remove origin
```

---

## 💾 4. Änderungen vorbereiten und committen

(Optional – nur falls du bereits etwas geändert hast.)

```bash
git add .
git commit -m "Initialize new project from template"
```

---

## ☁️ 5. Neues Repository auf GitHub erstellen

Auf GitHub:

- Name: **myNewProject**
- Sichtbarkeit: **Public**
- **README**, **.gitignore** und **License** **nicht hinzufügen**

---

## 🔗 6. Neue Remote-Verbindung herstellen

```bash
git remote add origin https://github.com/AgeVanBraun/myNewProject.git
```

---

## 🌿 7. Branch setzen und pushen

```bash
git branch -M main
git push -u origin main
```

---

# 🧩 GitHub Befehlsübersicht – Neues Projekt aus Template

| Nr. | Befehl                                                                  | Erklärung                                                                                                             |
| :-: | :---------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------- |
|  1  | `mkdir myNewProject`                                                    | Erstellt einen neuen lokalen Projektordner.                                                                           |
|  2  | `cd myNewProject`                                                       | Wechselt in den neu erstellten Ordner.                                                                                |
|  3  | `git clone https://github.com/AgeVanBraun/start-template.git .`         | Klont das Template-Repository direkt in den aktuellen Ordner (Punkt `.` verhindert das Erstellen eines Unterordners). |
|  4  | `git remote remove origin`                                              | Entfernt die alte Remote-Verbindung zum ursprünglichen Template-Repo.                                                 |
|  5  | `git add .`                                                             | Fügt alle geänderten oder neuen Dateien zur nächsten Commit-Vorbereitung hinzu.                                       |
|  6  | `git commit -m "Initialize new project from template"`                  | Erstellt einen Commit mit der Beschreibung des Projekts.                                                              |
|  7  | _(Auf GitHub neues Repo anlegen)_                                       | Neues Repository erstellen (**kein README**, **keine .gitignore**, **keine License**).                                |
|  8  | `git remote add origin https://github.com/AgeVanBraun/myNewProject.git` | Stellt die Verbindung zum neuen GitHub-Repository her.                                                                |
|  9  | `git branch -M main`                                                    | Setzt oder benennt den Hauptbranch in „main“ um (empfohlener Standard).                                               |
| 10  | `git push -u origin main`                                               | Lädt alle Dateien auf das neue GitHub-Repository hoch und verbindet lokale und entfernte Branches dauerhaft.          |

---

## ✅ Ergebnis

Dein neues Projekt **myNewProject** ist jetzt als eigenes Repository auf GitHub veröffentlicht –
basierend auf deinem Start-Template, aber mit sauberer Git-Historie und neuer Remote-Verbindung.
