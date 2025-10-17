# 🚀 Website Online Zetten - Stap voor Stap Handleiding

## Overzicht
Deze handleiding helpt je om de Nederlandse Verkiezingsanalyse website online te zetten via GitHub Pages.

## ✅ Wat is er al klaar?

1. ✅ Website bestanden zijn aangemaakt:
   - `index.html` - De hoofdpagina
   - `styles.css` - Styling voor de website
   - `script.js` - JavaScript functionaliteit

2. ✅ Automatische deployment is geconfigureerd:
   - `.github/workflows/deploy.yml` - GitHub Actions workflow voor automatische deployment

## 📋 Stappen om de Website Online te Zetten

### Stap 1: GitHub Pages Inschakelen

1. **Ga naar de GitHub repository**
   - Open: https://github.com/GH664527/nederlandse-verkiezingsanalyse

2. **Open Settings (Instellingen)**
   - Klik op de **Settings** tab bovenaan de repository pagina
   - ⚠️ Je moet admin rechten hebben op de repository

3. **Ga naar Pages**
   - Klik in het linker menu op **Pages** (onder "Code and automation")

4. **Configureer de Source**
   - Onder **Source**, selecteer **GitHub Actions**
   - Dit activeert de automatische deployment

5. **Wacht op de eerste deployment**
   - GitHub zal automatisch de workflow starten
   - Dit kan 1-2 minuten duren

### Stap 2: Controleer de Deployment

1. **Ga naar Actions tab**
   - Klik op de **Actions** tab in de repository
   - Je zou een workflow run moeten zien met de naam "Deploy Website to GitHub Pages"

2. **Wacht tot het groene vinkje verschijnt**
   - Groen vinkje ✅ = Deployment succesvol
   - Rood kruisje ❌ = Er is iets misgegaan (check de logs)

### Stap 3: Bezoek de Website

Zodra de deployment voltooid is, is de website beschikbaar op:

**URL:** `https://gh664527.github.io/nederlandse-verkiezingsanalyse/`

## 🔄 Updates Pushen

Vanaf nu werkt alles automatisch! Elke keer dat je wijzigingen pusht naar de `main` of `copilot/deploy-website-online` branch, wordt de website automatisch bijgewerkt.

### Workflow:
1. Maak wijzigingen in de HTML/CSS/JS bestanden
2. Commit en push de wijzigingen
3. GitHub Actions deploy automatisch de nieuwe versie
4. Na 1-2 minuten zijn je wijzigingen online zichtbaar

## 🛠️ Lokaal Testen

Voor je wijzigingen pusht, kun je ze lokaal testen:

### Optie 1: Direct openen
```bash
# Open index.html gewoon in je browser
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

### Optie 2: Lokale server (aanbevolen)
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (als je npx hebt)
npx http-server

# Bezoek dan: http://localhost:8000
```

## 📁 Bestandsstructuur

```
nederlandse-verkiezingsanalyse/
├── .github/
│   └── workflows/
│       └── deploy.yml          # Deployment configuratie
├── index.html                   # Hoofdpagina
├── styles.css                   # CSS styling
├── script.js                    # JavaScript
├── README.md                    # Project informatie
└── DEPLOYMENT_GUIDE.md         # Deze handleiding
```

## ❓ Veelgestelde Vragen

### Q: Hoe lang duurt het voor de website online staat?
A: Na het inschakelen van GitHub Pages, duurt de eerste deployment 1-2 minuten.

### Q: Kan ik een eigen domein gebruiken?
A: Ja! In de GitHub Pages settings kun je een custom domain configureren.

### Q: Hoe voeg ik meer pagina's toe?
A: Maak gewoon nieuwe HTML bestanden aan en link ernaar vanuit index.html.

### Q: De website werkt niet, wat nu?
A: 
1. Check of GitHub Pages is ingeschakeld (Settings → Pages)
2. Check of de workflow succesvol was (Actions tab)
3. Wacht een paar minuten en probeer opnieuw
4. Clear je browser cache

## 🎨 Website Aanpassen

### Kleuren wijzigen
Open `styles.css` en pas de kleuren in de header gradient aan:
```css
header {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

### Content wijzigen
Open `index.html` en pas de tekst aan in de verschillende secties.

### Nieuwe sectie toevoegen
Voeg een nieuwe `<section>` toe in `index.html`:
```html
<section>
    <h2>Jouw Titel</h2>
    <p>Jouw content hier...</p>
</section>
```

## 🔐 Beveiliging

De website is publiek toegankelijk. Zorg ervoor dat je:
- ❌ GEEN wachtwoorden of API keys in de code zet
- ❌ GEEN persoonlijke gegevens deelt
- ✅ Alleen publieke informatie publiceert

## 📞 Hulp Nodig?

Als je vastloopt:
1. Check de [GitHub Pages documentatie](https://docs.github.com/en/pages)
2. Check de [GitHub Actions logs](https://github.com/GH664527/nederlandse-verkiezingsanalyse/actions)
3. Open een issue in de repository

---

**Veel succes met je website! 🎉**
