# FinancePlus Mandato

Gestionale desktop offline per la creazione e l'archiviazione dei mandati di consulenza finanziaria FinancePlus.Tech.

## Funzioni principali

- anagrafica clienti;
- importazione di visure camerali e report PDF;
- estrazione automatica di denominazione, P.IVA/C.F., sede, PEC e amministratore;
- generazione di mandati Word dal modello `Mandato_vuoto.docx`;
- esportazione PDF tramite Microsoft Word o LibreOffice, quando installato;
- archivio locale SQLite;
- logo FinancePlus.Tech integrato.

## Avvio rapido su Windows

1. Installare Python 3.10 o superiore.
2. Scaricare o clonare il repository.
3. Fare doppio clic su `AVVIA_WINDOWS.bat`.

In alternativa, dal terminale:

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

## File principale

Il file da eseguire è:

```text
app.py
```

## Struttura

```text
FinancePlus_Mandato_GitHub/
├── app.py
├── Mandato_vuoto.docx
├── LOGO_FINANCE_2.PNG
├── requirements.txt
├── AVVIA_WINDOWS.bat
├── FinancePlus_Data/
│   ├── financeplus_mandato.db
│   └── financeplus_mandato.sqlite3
└── README.md
```

## Note

- L'applicazione è desktop Tkinter e non è una web app Streamlit.
- Per mantenere identico il layout del DOCX nel PDF è consigliato Microsoft Word oppure LibreOffice.
- I documenti generati e gli archivi locali vengono creati nella cartella `FinancePlus_Data`.
