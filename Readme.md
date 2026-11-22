<div align="center">
  <img src="./assets/icon.png" alt="Gestore Pedane" width="96" />

  # Gestore Pedane

  **La gestione digitale di movimentazioni, buoni pedane e contabilità vettori.**

  <p>
    Applicazione desktop progettata per semplificare il lavoro quotidiano:
    ordini, saldi cliente, fornitori, reportistica e dati sempre a portata di click.
  </p>

  <p>
    <a href="https://github.com/dolce95/gestione-pedane-releases/releases/latest/download/Gestore-Pedane-Setup-win-x64.exe">
      <img src="https://api.iconify.design/logos/microsoft-windows-icon.svg" width="15" height="15" valign="middle" alt="" />
      &nbsp;<strong>Scarica per Windows</strong>
    </a>
    &nbsp;&nbsp;|&nbsp;&nbsp;
    <a href="https://github.com/dolce95/gestione-pedane-releases/releases/latest/download/Gestore-Pedane-mac-arm64.zip">
      <img src="https://api.iconify.design/ri/apple-fill.svg?color=%2364748B" width="16" height="16" valign="middle" alt="" />
      &nbsp;<strong>Scarica per macOS</strong>
    </a>
  </p>

  <sub>
    <a href="https://github.com/dolce95/gestione-pedane-releases/releases">Versioni precedenti e note di rilascio</a>
  </sub>
</div>

---

## Funzionalità

- **Movimentazioni e saldi** — Registrazione degli ordini annuali e calcolo automatico dei saldi per cliente.
- **Buoni pedane** — Gestione dei buoni e riepiloghi dedicati per fornitore.
- **Anagrafica clienti e fornitori** — Informazioni operative organizzate in un'unica area di lavoro.
- **Report e solleciti** — Esportazione in PDF ed Excel con modelli personalizzabili e invio diretto tramite email.
- **I tuoi dati restano locali** — Database SQLite isolato nell'area utente del sistema.
- **Backup e ripristino** — Creazione di backup del database e ripristino dei dati quando necessario.
- **Aggiornamenti integrati** — Verifica e installazione delle nuove versioni dall'applicazione.

## Installazione

| Sistema | Requisiti | Procedura |
| :--- | :--- | :--- |
| ![Windows](https://api.iconify.design/logos/microsoft-windows-icon.svg?width=13) **Windows** | Windows 10 o 11, 64-bit | Apri l'installer `.exe` e completa la procedura guidata. |
| ![macOS](https://api.iconify.design/ri/apple-fill.svg?color=%2364748B&width=14) **macOS** | Apple Silicon (M1–M4) | Estrai il file `.zip`, quindi sposta `Gestore Pedane.app` in **Applicazioni**. |

<details>
<summary><strong>Avvisi di sicurezza al primo avvio</strong></summary>

#### Windows — Microsoft Defender SmartScreen

Se il sistema mostra un avviso, seleziona **Ulteriori informazioni** e poi **Esegui comunque**.

#### macOS — Gatekeeper

Se il sistema impedisce l'apertura dell'app, fai clic destro su `Gestore Pedane.app`, scegli **Apri** e conferma l'autorizzazione.

> Gli avvisi possono comparire quando un'applicazione desktop non è stata ancora riconosciuta dal sistema operativo.

</details>

## Aggiornamenti

Gestore Pedane controlla automaticamente la disponibilità di nuove versioni all'avvio.

Puoi verificare gli aggiornamenti manualmente da **Impostazioni → Aggiornamenti**.

## Privacy e dati

L'applicazione usa un database locale e non richiede l'uso di servizi cloud per la gestione ordinaria dei dati.

- Gli esportati e i backup vengono salvati nei percorsi configurati dall'utente.
- Le credenziali email, quando configurate, vengono utilizzate esclusivamente per l'invio dei report.
- Conserva una copia periodica del database su un supporto o in una posizione diversa dal computer principale.

## Sviluppo locale

### Requisiti

- Node.js
- npm

### Avvio in sviluppo

Apri due terminali nella cartella del progetto:

```bash
# Terminale 1
npm install
npm run dev

# Terminale 2
npm run electron
```

### Verifica e build

```bash
npm test
npm run lint
npm run build
```

### Pacchetti desktop

```bash
npm run dist:win
npm run dist:mac
```

Il progetto utilizza React, Vite, Electron e SQLite.

## Stack tecnico

- **Interfaccia:** React 19
- **Build frontend:** Vite 7
- **Applicazione desktop:** Electron 44
- **Database:** SQLite
- **Export:** PDF/Excel
- **Distribuzione:** electron-builder e GitHub Releases
