# Tirocini DSS — Come fare un tirocinio

Sito statico (HTML + CSS, nessuna dipendenza né build) con le istruzioni per i tirocini del Dipartimento di Scienze Statistiche, Sapienza. Pronto per GitHub Pages.

## Pubblicare su GitHub Pages

1. Crea un repository (ad esempio `internship-dss`) e carica il contenuto di questa cartella nella radice.
2. Su GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, cartella `/ (root)`.
3. Dopo un minuto il sito è online su `https://<utente-o-organizzazione>.github.io/internship-dss/`.

Il file `.nojekyll` disattiva Jekyll: GitHub serve le pagine così come sono. Tutti i link interni sono relativi, quindi il sito funziona sia come project page sia con un dominio personalizzato.

## Anteprima in locale

```bash
python3 -m http.server 8000
# poi apri http://localhost:8000
```

## Struttura

| File | Contenuto |
|---|---|
| `index.html` | Home con i cinque passi |
| `informati.html`, `scegli.html`, `formalizza.html`, `fai.html`, `valida.html` | I cinque passi |
| `chi-e-chi.html` | Attori della procedura |
| `aziende.html` | Istruzioni per gli enti ospitanti |
| `faq.html` | Domande frequenti |
| `assets/style.css` | Stile (con tema scuro automatico) |

Per modificare il testo basta aprire il file HTML della pagina: l'intestazione e il piè di pagina sono ripetuti in ogni file.

## Screenshot TSP

Per ora il sito è solo testo. Quando la copertura sarà completa, metti le immagini in `assets/img/` e inseriscile con `<img src="assets/img/NOMEFILE.png" alt="…">`. Prima della pubblicazione oscura i dati personali (codice fiscale, indirizzo, data di nascita, firme) negli screenshot del Progetto Formativo.

Abbinamento suggerito (nomi dei file già usati nelle cartelle Drive):

| Pagina | Screenshot |
|---|---|
| Scegli | `TSP_CV_*`, `TSP_RicercaEnteOspitante_*`, `TSP_RicercaOpportunita_*`, `TSP_Opportunita_*` |
| Formalizza | `TSP_Autocandidatura_*`, `TSP_ProgettoFormativo_*`, `TSP_MieiTirocini_StatoPFAttivato.png` |
| Fai | `TSP_PeriodiTirocinio_RegistroPresenzeInBozza.png`, `TSP_Periodi_RegistroPresenzeApprovato.png` |
| Valida | `TSP_Valutazione_QuestionarioCompilatoERelazioneFinale.png`, `TSP_MieiTirocini_TirocinioChiusoPFConcluso.png` |

## Da completare / da confermare

- Link «Post Internship Day per gli studenti» (presente nella vecchia bozza, mai completato).
- Screenshot mancanti: login, accreditamento enti, invio del registro presenze, questionario di valutazione e di monitoraggio, relazione finale, chiusura del tirocinio.
