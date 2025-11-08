
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

*(`DEINNAME` & `meinProjekt` anpassen)*

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

| Befehl              | Bedeutung                                      |
|---------------------|------------------------------------------------|
| `git init`          | Git starten                                    |
| `git add .`         | alle Änderungen vormerken                      |
| `git commit -m ""`  | Änderung benennen und speichern                |
| `git push`          | Hochladen zu GitHub                            |
| `git branch`        | zeigt aktuellen Branch                         |
| `git remote add`    | Verbindung zu GitHub herstellen                |

---

📁 **Tipp**: Diese Datei kannst du in jedem Projekt speichern, z. B. als:

```bash
git-cheatsheet.md
```

Dann hast du immer deine eigene Hilfe zur Hand ✅
