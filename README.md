# 🏃 RunTrack Pro

PWA per la preparazione alla corsa — maratona, mezza maratona, 25km e 10km.

## ✨ Funzionalità

- **4 piani di allenamento**: Maratona (16 sett.), Mezza Maratona (12 sett.), 25km (10 sett.), 10km (8 sett.)
- **Tabella settimanale** organizzata per mese con sessioni dettagliate
- **Registrazione allenamenti**: km, durata, bpm, note
- **Statistiche**: km totali, pace migliore, streak, progressione piano
- **Calcolatore pace**
- **Funziona offline** (Service Worker)
- **Installabile su iPhone** come app nativa

---

## 🚀 Installazione su GitHub Pages

### 1. Crea repository su GitHub

```bash
git init
git add .
git commit -m "Initial commit - RunTrack Pro"
git branch -M main
git remote add origin https://github.com/TUO_USERNAME/runtrack-pro.git
git push -u origin main
```

### 2. Abilita GitHub Pages

1. Vai su **Settings** del repository
2. Sezione **Pages**
3. Source: **Deploy from a branch** → `main` → `/ (root)`
4. Clicca **Save**
5. L'app sarà disponibile su: `https://TUO_USERNAME.github.io/runtrack-pro`

---

## 📲 Installazione su iPhone 13 Pro Max

1. Apri **Safari** (obbligatorio, non Chrome)
2. Vai sull'URL di GitHub Pages
3. Tocca il bottone **Condividi** (quadrato con freccia in su)
4. Scorri e tocca **"Aggiungi a schermata Home"**
5. Tocca **Aggiungi**

L'app apparirà come icona sulla schermata home e funzionerà **senza connessione internet**.

---

## 📁 Struttura file

```
runtrack-pro/
├── index.html      ← App completa (HTML + CSS + JS)
├── manifest.json   ← Configurazione PWA
├── sw.js           ← Service Worker (offline)
├── icon-192.png    ← Icona app
├── icon-512.png    ← Icona app HD
└── README.md
```

---

## 🗂 Zone di intensità (Z)

| Zona | Descrizione | % FC Max |
|------|-------------|----------|
| Z1 | Recupero attivo | 50-60% |
| Z2 | Aerobico base (facile) | 60-70% |
| Z3 | Aerobico (soglia aerobica) | 70-80% |
| Z4 | Soglia anaerobica | 80-90% |
| Z5 | Massimale | 90-100% |

---

## 💾 Dati

Tutti i dati vengono salvati localmente sul dispositivo tramite `localStorage`. Non serve account o server.
