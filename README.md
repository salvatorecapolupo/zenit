Ecco un file `README.md` strutturato per documentare l'evoluzione del progetto, analizzando il processo iterativo e le versioni che abbiamo attraversato.

---

# 💸 zenit 
### *The Retro-CLI Financial Forecaster*

`zenit` è un simulatore finanziario deterministico a 90 giorni. Nato dalla necessità di eliminare la burocrazia delle app di budgeting moderne, trasforma la gestione del denaro in un'interfaccia a riga di comando (CLI) ispirata alle avventure grafiche anni '90.

---

## 🇮🇹 Versione Italiana

### 🚀 Evoluzione del Progetto
Il percorso di sviluppo è stato un processo iterativo di "sottrazione": siamo partiti da un'interfaccia complessa per arrivare alla purezza del terminale.

#### Fase 1: La Dashboard Tradizionale (L'errore)
* **Versioni:** v1.0 e v2.0.
* **Prompt Utente:** *"vorrei simulare... rendi l'istogramma verde se attivo e rosso se passivo"*.
* **Difetti:** Troppa UI, bottoni ingombranti, gestione dell'input lenta. L'utente l'ha definita "poco usabile".

#### Fase 2: L'Ispirazione Monkey Island (La svolta)
* **Versione:** v3.0 (Monkey Island Style).
* **Prompt Utente:** *"facciamolo da console... coi bottoni di Monkey Island 2"*.
* **Innovazione:** Introduzione della macchina a stati per l'input e della console testuale.
* **Bug rilevati:** L'interfaccia era ancora "fragile" (l'input non scriveva correttamente) e il grafico aveva una crescita esponenziale errata.

#### Fase 3: CLI Pura e Tag Interattivi (La forma finale)
* **Versioni:** v3.5 e Final.
* **Prompt Utente:** *"interfaccia a linea di comando... comandi in italiano... i comandi giusti diventano tag editabili"*.
* **Soluzione:** Rimozione di ogni menu. Inserimento tramite verbi (`SALDO`, `FISSO`, `SPESA`). I dati diventano "oggetti" (Tag) cancellabili e modificabili con un click.

### 🛠 Comandi Supportati
* `SALDO [cifra]`: Imposta il punto di partenza.
* `FISSO [giorno] [cifra]`: Ricorrenza mensile (es. stipendio o affitto).
* `SPESA [gg/mm] [cifra]`: Evento singolo (es. acquisto smartphone).
* `RESET`: Pulisce la memoria.

---

## 🇬🇧 English Version

### 🚀 Project Evolution
The development was a process of "subtraction": moving away from heavy UI towards the efficiency of a raw terminal.

#### Phase 1: The Traditional Dashboard (The Mistake)
* **Versions:** v1.0 & v2.0.
* **User Prompt:** *"I want to simulate... make the histogram green if positive and red if negative"*.
* **Flaws:** Clunky UI, slow input management. User feedback: "not very usable."

#### Phase 2: Monkey Island Inspiration (The Pivot)
* **Version:** v3.0 (Monkey Island Style).
* **User Prompt:** *"let's do it via console... with Monkey Island 2 buttons"*.
* **Innovation:** Introduction of a State Machine for inputs and a scrolling text log.
* **Bugs:** Input focus issues and a logic error causing a "fake" exponential growth in the chart.

#### Phase 3: Pure CLI & Interactive Tags (Final Form)
* **Versions:** v3.5 & Final.
* **User Prompt:** *"command line interface... commands in Italian... valid commands become editable tags"*.
* **Solution:** All menus removed. Data entry via verbs (`SALDO`, `FISSO`, `SPESA`). Data points are converted into interactive "Tags" that can be edited or deleted with a click.

### 🛠 Supported Commands
* `SALDO [amount]`: Sets the starting balance.
* `FISSO [day] [amount]`: Monthly recurring (e.g., salary/rent).
* `SPESA [dd/mm] [amount]`: One-time event (e.g., buying a phone).
* `RESET`: Clears all data.

---

## 📊 Technical Analysis / Analisi Tecnica

| Feature | Description |
| :--- | :--- |
| **Logic** | Deterministic 90-day projection (No AI, pure math). |
| **Graphics** | Mirrored Histogram (Positive up/Green, Negative down/Red). |
| **UX** | Focus-first CLI. Commands are parsed and ignored if invalid. |
| **Architecture** | Single-file HTML/JS (No dependencies). |

---

> **Note:** "zenit" is not just an app, it's a workflow for people who think in commands.
