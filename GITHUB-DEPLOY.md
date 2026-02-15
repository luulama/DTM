# GitHub Pages Deployment Guide

## Steg 1: Skapa GitHub Repository

1. Gå till https://github.com
2. Klicka "New repository"
3. Namnge: `dpm-workbench`
4. Välj "Public"
5. Klicka "Create repository"

## Steg 2: Ladda upp filen

### Via GitHub Web Interface (Enklast):

1. I ditt nya repo, klicka "uploading an existing file"
2. Dra `DPM-EDITABLE.html` till sidan
3. Döp om till `index.html` (viktigt!)
4. Klicka "Commit changes"

### Via Git (Terminal):

```bash
# Gå till mappen där DPM-EDITABLE.html finns
cd ~/Downloads

# Kopiera och döp om filen
cp DPM-EDITABLE.html index.html

# Initiera Git
git init
git add index.html
git commit -m "Initial commit"

# Koppla till ditt repo (ersätt USERNAME)
git remote add origin https://github.com/USERNAME/dpm-workbench.git
git branch -M main
git push -u origin main
```

## Steg 3: Aktivera GitHub Pages

1. I ditt repo, gå till "Settings"
2. Klicka "Pages" (vänster meny)
3. Under "Source", välj "main" branch
4. Klicka "Save"
5. Vänta 1-2 minuter

## Steg 4: Få din länk

Din webbplats finns nu på:
```
https://USERNAME.github.io/dpm-workbench/
```

Ersätt USERNAME med ditt GitHub-användarnamn.

## Uppdatera filen:

1. Gå till ditt repo
2. Klicka på `index.html`
3. Klicka pennikonen (Edit)
4. Klistra in ny kod
5. Klicka "Commit changes"
6. Vänta 30 sekunder - sidan uppdateras automatiskt

## Tips:

- Länken fungerar på ALLA datorer
- localStorage sparas per webbläsare
- Gratis och obegränsat
- HTTPS säkert
- Uppdateras automatiskt vid ny commit

## Support:

GitHub Pages dokumentation:
https://docs.github.com/en/pages
