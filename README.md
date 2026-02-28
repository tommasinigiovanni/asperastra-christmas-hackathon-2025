# 🎄 AstraGPT - AI Mentor per Hackathon

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with AI](https://img.shields.io/badge/Made%20with-AI%20%E2%9D%A4%EF%B8%8F-ff69b4)](https://evoseed.io)
[![Hackathon](https://img.shields.io/badge/Event-Christmas%20Hackathon%202025-red?logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9IndoaXRlIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCI+PHBhdGggZD0iTTEyIDJMNiAxMmg0djEwaDRWMTJoNHoiLz48L3N2Zz4=)](https://www.eventbrite.it/e/christmas-hackathon-tickets-1963193523677)
[![Location](https://img.shields.io/badge/Location-Trieste%20🇮🇹-green)](https://asperastra.com)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)

Una **Single Page Application** che simula un'interfaccia ChatGPT per presentazioni interattive dal vivo. Sviluppata per guidare i team durante il **Christmas Hackathon AsperAstra 2025** con metodologia **Pretotyping**.

🔗 **Repository:** https://github.com/tommasinigiovanni/asperastra-christmas-hackathon-2025

📄 **Scarica il PDF:** [2025-12_AI-Mentor_Hackathon-AsperAstra.pdf](./2025-12_AI-Mentor_Hackathon-AsperAstra.pdf)

---

## 🎯 Cos'è AstraGPT?

**AstraGPT** è un AI Mentor virtuale che guida i partecipanti dell'hackathon attraverso le fasi cruciali:

- 📋 **Definizione del problema** con A3 Canvas
- 🧪 **Pretotyping** prima di prototipare (con esempio Fireflies.ai!)
- 📊 **Validazione** con Ipotesi XYZ
- 🛠️ **Tool selection** No-Code & AI
- 📝 **Lean Canvas** per il business model
- 🎤 **Pitch** structure

> *"Pretotipare prima di prototipare. Fatto è meglio che perfetto."*

---

## 🚀 Quick Start

### Con Docker (Raccomandato)

```bash
# Build e run
docker build -t astragpt .
docker run -d -p 8080:80 astragpt

# Apri nel browser
open http://localhost:8080
```

### Con Docker Compose (Dev mode)

```bash
docker compose up
open http://localhost:8080
```

### Senza Docker

```bash
# Con Python
python3 -m http.server 8080

# Con Node.js
npx http-server -p 8080
```

---

## ⌨️ Controlli

| Tasto | Azione |
|-------|--------|
| **INVIO / SPAZIO / →** | Avanti |
| **←** | Indietro |
| **H** | Nascondi UI (Stealth Mode) |
| **R** | Reset presentazione |
| **P** | Modalità Presentatore |

---

## 📁 Struttura Progetto

```
.
├── index.html            # Pagina principale
├── src/                  # 📦 Codice sorgente
│   ├── script-content.js # 📝 COPIONE - modifica qui i contenuti!
│   ├── config.js         # Configurazione
│   ├── main.js           # Controller principale
│   ├── animation-engine.js # Animazioni e effetti
│   ├── chat-manager.js   # Gestione messaggi
│   ├── state-manager.js  # Gestione stato
│   └── style.css         # Stili (tema ChatGPT dark)
├── img/                  # Immagini (A3, Lean Canvas, ecc.)
├── Dockerfile            # Build produzione
└── docker-compose.yml    # Dev environment
```

---

## ✏️ Personalizza il Copione

Modifica `src/script-content.js` per adattare la presentazione:

```javascript
const SCRIPT = [
    {
        role: 'user',
        text: "La tua domanda...",
        notes: "Note per te (visibili in Presenter Mode)"
    },
    {
        role: 'ai',
        text: "Risposta di AstraGPT...",
        sound: 'ding',           // Effetto sonoro
        effect: 'sparkle',       // Effetto visivo
        buttons: [               // Bottoni per branching
            { label: "Opzione A", nextIndex: 5 },
            { label: "Opzione B", nextIndex: 8 }
        ]
    }
];
```

### Effetti Disponibili

| Suoni | Effetti Visivi |
|-------|----------------|
| `'startup'` - Boot AI | `'confetti'` - Coriandoli |
| `'ding'` - Campanello | `'sparkle'` - Stelline |
| `'glitch'` - Allarme | `'highlight'` - Flash |
| `'applause'` - Applausi | |

---

## 🎯 Filosofia

> *"L'AI è un moltiplicatore: 0 × AI = 0. Ma voi non siete zero."*

> *"Prima vendi, poi automatizza."* - Lezione da Fireflies.ai

> *"Good enough for now, safe enough to try."*

---

## ✨ Features

- 🎨 **Interfaccia ChatGPT** - Clone pixel-perfect tema scuro
- ⌨️ **Typing Animation** - Simulazione realistica carattere per carattere
- 🔀 **Branching Logic** - Bivi narrativi con bottoni
- 🔊 **Sound Effects** - Suoni generati con Web Audio API
- ✨ **Visual Effects** - Confetti, sparkle, highlight
- ❄️ **Snow Effect** - Neve natalizia sui bordi
- 📱 **Responsive** - Mobile, tablet, desktop
- ♿ **Accessibile** - WCAG 2.1 AA compliant
- 💾 **Persistenza** - Salvataggio automatico stato
- 🐳 **Docker Ready** - Container ottimizzato < 40MB

---

## 👨‍💻 Autore

<a href="https://www.linkedin.com/in/giovannitommasini/">
  <img src="https://img.shields.io/badge/LinkedIn-Giovanni%20Tommasini-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="https://www.giovannitommasini.it/">
  <img src="https://img.shields.io/badge/Website-giovannitommasini.it-FF5722?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website">
</a>
<a href="https://evoseed.io">
  <img src="https://img.shields.io/badge/Company-Evoseed.io-00C853?style=for-the-badge&logo=seedling&logoColor=white" alt="Evoseed">
</a>
<a href="https://instagram.com/tommasini.giovanni">
  <img src="https://img.shields.io/badge/Instagram-tommasini.giovanni-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
</a>
<a href="https://t.me/tommasinigiovanni">
  <img src="https://img.shields.io/badge/Telegram-tommasinigiovanni-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
</a>
<a href="https://github.com/tommasinigiovanni">
  <img src="https://img.shields.io/badge/GitHub-tommasinigiovanni-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
</a>

**Giovanni Tommasini** - Telco & AI DevOps Expert | CTO @ AI Fabric | Co-founder @ Evoseed

> *"Enthusiastic Seeker"* 🔍 - Ottimizzazione processi attraverso automazione e AI.

🎙️ **Podcast:** *Uno Nessuno Centomil AI* - su [YouTube](https://www.youtube.com/@unonessuno100milai) e [Spotify](https://open.spotify.com/show/unonessuno100milai)

---

## 🙏 Acknowledgments

- **Alberto Savoia** per la metodologia Pretotyping
- **OpenAI** per l'ispirazione UI ChatGPT
- **AsperAstra** per l'opportunità dell'hackathon
- **Fireflies.ai** per l'esempio di pretotipo perfetto

---

## 📄 Licenza

MIT - Usa, modifica e condividi liberamente!

---

<div align="center">

Made with ❤️ by [Giovanni Tommasini](https://linkedin.com/in/giovannitommasini) per il **Christmas Hackathon AsperAstra 2025** 🎄

**[⬆ Torna su](#-astragpt---ai-mentor-per-hackathon)**

</div>
