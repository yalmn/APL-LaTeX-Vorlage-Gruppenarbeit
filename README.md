# APL LaTeX-Vorlage (Gruppenarbeit)

Diese Vorlage dient als Grundlage für wissenschaftliche Arbeiten, Projektberichte oder APL-Gruppenarbeiten.  
Sie ist modular aufgebaut und kann sowohl **in Overleaf** als auch **lokal mit TeX Live oder MiKTeX** verwendet werden.

---

## Arbeiten mit Forks und Branches

Gerne könnt ihr auch Veränderungen über einen **Fork** des Projekts vornehmen.  
Folgt dazu diesem Ablauf:

1. **Repository forken** (auf GitHub: „Fork“ klicken)
2. **Eigenen Fork klonen**
   ```bash
   git clone https://github.com/<dein-username>/<repo-name>.git
   cd <repo-name>
   ```
3. **Upstream zum Original hinzufügen** (optional, aber empfohlen)
   ```bash
   git remote add upstream https://github.com/<original-owner>/<repo-name>.git
   git fetch upstream
   ```
4. **Neuen Branch erstellen**
   ```bash
   git checkout -b feature/meine-aenderung
   ```
5. **Änderungen vornehmen und committen**
   ```bash
   git add .
   git commit -m "Beschreibung der Änderung"
   ```
6. **Branch in deinen Fork pushen**
   ```bash
   git push origin feature/meine-aenderung
   ```
7. **Pull Request erstellen** (auf GitHub: „Compare & pull request“)

> So bleibt der `main`-Branch stabil und alle Änderungen nachvollziehbar.

---

## Schnellstart

### In Overleaf
1. Lade das **letzte Release** herunter.  
2. Lade die `.zip`-Datei in **Overleaf** hoch.  
3. Öffne das Projekt und starte direkt mit der Bearbeitung.  

### Lokal mit LaTeX
```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

---


## Projektstruktur

```
APL_Vorlage_Gruppenarbeit/
├── appendix/                # Anhangsdateien
│   └── appendix_a.tex
├── bib/                     # Literaturverzeichnis (BibTeX)
│   └── references.bib
├── contents/                # Hauptinhalte der Arbeit
│   ├── abkuerzungen.tex     # Abkürzungsverzeichnis
│   ├── abstract.tex         # Abstract / Kurzfassung
│   ├── affirmation.tex      # Eigenständigkeitserklärung
│   ├── introduction.tex     # Einleitung
│   └── restriction.tex      # Sperrvermerk (optional)
├── figures/                 # Abbildungen
│   └── beispielbild.png
├── includes/                # Strukturelle Dateien
│   ├── authors.tex          # Autorenangaben
│   ├── header.tex           # Kopfzeilen / Titelseite
│   ├── meta.tex             # Meta-Informationen (Titel, Betreuer, etc.)
│   └── packages.tex         # Eingebundene LaTeX-Pakete
└── main.tex                 # Haupteinstiegspunkt des Dokuments
```

---

## Features

- IEEE-Zitierstil (`\cite{}` einheitlich verwendbar)  
- Saubere Trennung von **Inhalt** und **Struktur**  
- Anpassbares **Titelseitenlayout**  
- Übersichtliches **Abkürzungsverzeichnis**  
- Unterstützung für **mehrere Autoren und Betreuer**  
- **Anhang** mit separaten `.tex`-Dateien  
- Beispielabbildung (`beispielbild.png`) enthalten  

---

## Zitierweise

Diese Vorlage nutzt den **IEEE-Zitierstil**.  
Beispiel:  
```latex
Wie in \cite{sampleReference} beschrieben, ...
```
Einträge werden in `bib/references.bib` verwaltet.

---

## Autoren und Nutzung

Diese Vorlage wurde erstellt, um Gruppenarbeiten und wissenschaftliche Projekte effizient zu strukturieren.  
Sie kann frei angepasst, erweitert und geteilt werden.
