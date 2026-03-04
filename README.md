# Portfolio Sara Stabucchi

Sito web personale professionale realizzato per presentare progetti, competenze e servizi di sviluppo web.

## Indirizzo Online

**GitHub Pages**: https://francescopaganotustena-hash.github.io/MioSito/

## Struttura del Progetto

```
SitoWeb/
├── index.html                    # Homepage principale
├── progetto-neuralflow.html      # Progetto 1: AI Workflow Automation
├── progetto-ecotracker.html      # Progetto 2: Monitoraggio Ambientale
├── progetto-virtuspace.html      # Progetto 3: Realtà Virtuale
├── progetto-codeforge.html       # Progetto 4: Sviluppo Software
├── css/
│   ├── style.css                 # Stili tema scuro principale
│   └── project.css               # Stili pagine progetto
├── js/
│   └── main.js                   # Script: smooth scroll, animazioni, form contatti
└── img/
    ├── foto.jpg                  # Foto profilo
    └── favicon.svg               # Icona sito (I&S)
```

## Caratteristiche Implementate

### Homepage
- **Hero**: Intro con nome e tagline
- **Progetti**: 4 schede progetto con link alle pagine dettagliate
- **Chi sezione "Chi sono"**: Foto profilo, bio, competenze tecniche
- **Contatti**: Form funzionante con integrazione Formspree

### Pagine Progetto
Ogni pagina progetto contiene:
- Titolo e descrizione completa
- Tecnologie utilizzate
- Link al sito live (dove disponibile)
- Footer con copyright

### Funzionalità JavaScript
- Smooth scroll per navigazione
- Animazioni fade-in all scroll (IntersectionObserver)
- Hamburger menu mobile
- Active state navigazione durante scroll
- Header shadow allo scroll
- Form contatti con invio AJAX via Formspree

### Design
- Tema scuro moderno
- Colore primario: cyan (#00d4ff)
- Colore secondario: viola (#a78bfa)
- Font: Inter (Google Fonts)
- Responsive design
- Accessibilità: skip-to-content, aria-label, focus styles

### SEO e Meta
- Meta description e keywords
- Open Graph tags per social
- Twitter Card
- Lazy loading immagini
- Favicon SVG

## Configurazione Form Contatti

Il form utilizza **Formspree** per l'invio email senza backend.

### Setup Formspree
1. Registrati su [formspree.io](https://formspree.io)
2. Crea un nuovo form
3. Copia l'ID del form
4. Modifica `index.html` riga 176:
   ```html
   action="https://formspree.io/f/TUO_FORM_ID"
   ```

## Esecuzione Locale

### Server HTTP Python
```bash
cd /home/sviluppatore/Documenti/SitoWeb
python3 -m http.server 8000
```
Poi apri: http://localhost:8000

### Server HTTP Node.js
```bash
npx serve .
```

## Deploy su GitHub Pages

1. Repository già configurato su GitHub
2. Vai su Settings → Pages del repository
3. Source: Deploy from a branch → Branch: main → Folder: / (root)
4. Salva e attendi 1-2 minuti
5. Il sito sarà disponibile all'indirizzo del repository

## Comandi Git

### Configurazione iniziale (già fatto)
```bash
git config --global user.email "francescopagano.tustena@gmail.com"
git config --global user.name "Francesco Pagano"
git remote add origin git@github.com:francescopaganotustena-hash/MioSito.git
```

### Commit e Push
```bash
# Aggiungi tutti i file modificati
git add -A

# Crea commit con messaggio
git commit -m "Descrizione delle modifiche"

# Push su GitHub
git push
```

### Pull (scaricare modifiche)
```bash
git pull origin main
```

### Verifica stato
```bash
git status
git log --oneline
```

## Commit Recenti

| Data | Descrizione |
|------|-------------|
| 2026-03-04 | Sostituzione nome con Sara Stabucchi |
| 2026-03-04 | Logo FP → Innovation & Security |
| 2026-03-04 | Correzione genere femminile nel testo |
| 2026-03-04 | Nuova foto profilo |
| 2026-03-04 | Traduzione "About" → "Chi sono" |
| 2026-03-04 | Integrazione Formspree per form contatti |

## Note Future

- Aggiornare i link ai siti live dei progetti quando disponibili
- Aggiungere altri progetti man mano che vengono realizzati
- Considerare l'aggiunta di un blog o sezione articoli
- Valutare l'uso di un dominio personalizzato

## Tech Stack

- **HTML5** - Struttura semantica
- **CSS3** - Stili con variabili CSS, flexbox, grid
- **JavaScript** - Vanilla JS (no framework)
- **Git** - Versionamento
- **GitHub Pages** - Hosting gratuito
- **Formspree** - Gestione form contatti