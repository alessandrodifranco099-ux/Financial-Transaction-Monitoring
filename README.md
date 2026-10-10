# Financial Transaction Monitoring

> **Excel & Power BI Project** | Data Quality, Rules Engine & Risk Visualisation

---

## 🇮🇹 Presentazione del Progetto (Italiano)
Questo progetto nasce con l'obiettivo di simulare un processo reale di **monitoraggio delle transazioni finanziarie e controllo dei rischi operativi**. 

Attraverso l'integrazione tra un motore logico strutturato su **Microsoft Excel** e un cruscotto visivo su **Power BI**, il modello automatizza l'individuazione di anomalie (superamento soglie di legge, schemi di frazionamento sotto soglia e paesi a rischio), assegnando uno scoring di priorità e un'azione operativa immediata (Blocco o Monitoraggio).

---

## 🇬🇧 Project Overview (English)
This project simulates an operational workflow for **financial transaction monitoring and risk control**.

Combining a logic and validation engine built in **Microsoft Excel** with an interactive **Power BI** dashboard, the solution automates the detection of suspicious patterns (threshold breaches, transaction structuring/smurfing, and high-risk jurisdictions). Each transaction is assigned an objective risk score and a clear operational next step (Block, Review, or Approved).

---

## 📊 Dashboard Preview
![Dashboard Preview](dashboard_preview.png)
<img width="1441" height="808" alt="Dashboard_Preview" src="https://github.com/user-attachments/assets/56972b9b-e7ba-44c2-8659-2cbd8e50e66d" />


---

## ⚙️ Come è Strutturato il Progetto

### 1. Modello Logico (Excel)
- **Foglio `Regole`**: Tabella di governance separata contenente i parametri operativi (soglie di importo a 10.000 €, perimetro di frazionamento tra 9.500 € e 10.000 €, lista dei paesi a rischio).
- **Foglio `Transazioni`**: Dataset operativo con controlli automatizzati tramite formule nidificate (`SE`, `E`, `CONFRONTA`, `VAL.NUMERO`).
- **Scoring & Workflow**: Assegnazione dinamica del livello di rischio (**Basso**, **Medio**, **Alto**) e della conseguente azione operativa (**Blocco & SOS**, **Monitoraggio**, **Nessuna**).
- **Foglio `Dashboard`**: Sintesi esecutiva con conteggi dinamici (`CONTA.SE`) e distribuzioni percentuali.

### 2. Cruscotto Interattivo (Power BI)
- **Schede KPI**: Monitoraggio immediato del volume transato totale (€ 98K) e del conteggio delle operazioni (15).
- **Donut Chart**: Ripartizione percentuale e volumetrica del rischio.
- **Bar Chart per Giurisdizione**: Visualizzazione dell'esposizione finanziaria per singolo Paese di controparte.
- **Filtro Dinamico (Slicer)**: Possibilità di isolare con un clic solo le posizioni che richiedono intervento operativo.

---

## 📁 File Inclusi
- `Financial_Transaction_Monitoring.xlsx`: Cartella di lavoro completa con dataset, regole e formule.
- `Financial_Transaction_Monitoring.pbix`: Report interattivo Power BI Desktop.
