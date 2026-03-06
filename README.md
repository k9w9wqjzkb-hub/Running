# 🏃 RunCoach — Piano di Allenamento per la Corsa

PWA (Progressive Web App) per la preparazione di gare podistiche: Maratona, Mezza Maratona, 25Km, 10Km.

## ✨ Funzionalità

- **4 piani di allenamento**: Maratona (16 sett.), Mezza (12 sett.), 25Km (10 sett.), 10Km (8 sett.)
- **Tabelle mensili** con sessioni settimanali dettagliate
- **Tipi di allenamento**: Corsa Leggera, Tempo, Lungo, Intervalli, Recupero
- **Diario allenamenti**: registra km, tempo, tipo e note per ogni sessione
- **Statistiche**: km totali, sessioni, media, ritmo migliore
- **Grafico km settimanali**
- **Calcolatore passo** (min/km da distanza + tempo obiettivo)
- **Offline completo** grazie al Service Worker
- **Installabile su iPhone** (e qualsiasi dispositivo mobile)

---

## 🚀 Deploy su GitHub Pages

### Passo 1 — Crea il repository

```bash
git init
git add .
git commit -m "Initial commit: RunCoach PWA"
```

### Passo 2 — Crea repo su GitHub

1. Vai su [github.com/new](https://github.com/new)
2. Nome repository: `runcoach` (o quello che preferisci)
3. Visibilità: **Public** (necessario per GitHub Pages gratuito)
4. Clicca **Create repository**

### Passo 3 — Push del codice

```bash
git remote add origin https://github.com/TUO_USERNAME/runcoach.git
git branch -M main
git push -u origin main
```

### Passo 4 — Attiva GitHub Pages

1. Nel tuo repository → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `/ (root)`
4. Clicca **Save**
5. Aspetta 1-2 minuti → la tua app sarà su:
   `https://TUO_USERNAME.github.io/runcoach/`

---

## 📱 Installazione su iPhone 13 Pro Max

1. Apri **Safari** (obbligatorio su iOS)
2. Vai su `https://TUO_USERNAME.github.io/runcoach/`
3. Tocca il pulsante **Condividi** (rettangolo con freccia su)
4. Scorri e tocca **"Aggiungi a schermata Home"**
5. Dai un nome (es. "RunCoach") → **Aggiungi**

L'app apparirà come icona nella home del tuo iPhone e si aprirà a schermo intero, **senza barra del browser**.

### ✅ Funziona offline?
Sì! Dopo la prima apertura con connessione, l'app funziona completamente offline grazie al Service Worker. I tuoi dati (allenamenti registrati) sono salvati nel localStorage del browser e persistono tra le sessioni.

---

## 📁 Struttura file

```
runcoach/
├── index.html      # App completa (HTML + CSS + JS tutto-in-uno)
├── manifest.json   # Configurazione PWA
├── sw.js           # Service Worker per offline
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── README.md
```

---

## 🛠️ Sviluppo locale

```bash
# Con Python (già installato su Mac/Linux)
python3 -m http.server 8080

# Poi apri: http://localhost:8080
```

> ⚠️ Il Service Worker funziona solo su HTTPS o localhost.

---

## 📊 Piani di allenamento inclusi

| Gara | Settimane | Sessioni/settimana | Km max lungo |
|------|-----------|-------------------|-------------|
| Maratona 42Km | 16 | 4 | 32 km |
| Mezza Maratona 21Km | 12 | 4 | 20 km |
| 25 Km | 10 | 3 | 22 km |
| 10 Km | 8 | 3 | 10 km |

---

## 🔒 Privacy

Tutti i dati (allenamenti, progressi) sono salvati **localmente sul tuo dispositivo** nel browser. Nessun dato viene inviato a server esterni.
