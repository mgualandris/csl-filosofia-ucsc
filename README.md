# Stili CSL per Zotero: tesi di Filosofia (UCSC)

Due stili CSL per Zotero che producono note a piè di pagina e bibliografia secondo le norme redazionali del Dipartimento di Filosofia dell'Università Cattolica del Sacro Cuore (Milano).

Non è uno strumento ufficiale dell'Università. Le norme redazionali restano quelle del Dipartimento e del proprio relatore: in caso di dubbio prevalgono sempre le loro indicazioni.

## Quale file scegliere

| File | Quando usarlo |
|---|---|
| `ucsc-filosofia.csl` | Indicazioni principali delle norme. Autori in tondo, bibliografia con il nome dell'autore ripetuto. |
| `ucsc-filosofia-maiuscoletto.csl` | Indicazioni alternative. Autori e curatori in maiuscoletto, trattino lungo al posto del nome per le opere successive dello stesso autore. |

## Installazione

1. Scarica il file `.csl` che ti serve (apri il file su GitHub, poi "Download raw file").
2. In Zotero apri le impostazioni, sezione "Cita", scheda "Stili", e premi il pulsante "+" per aggiungere un file di stile. In alternativa trascina il file `.csl` sulla finestra di Zotero.
3. Nel plugin di Word seleziona lo stile e, come lingua del documento, "Italiano" oppure "predefinita dello stile".

## Compilare le voci

Lo stile funziona solo se i campi di Zotero sono compilati nel modo previsto: alcuni dati vanno scritti nel campo "Extra" o in campi particolari (traduttore e curatore, edizione, opere in più volumi, in corso di stampa, atti di convegno, fonti web). Tutte le regole sono nel file [`docs/regole-di-utilizzo.md`](docs/regole-di-utilizzo.md): è breve, leggilo prima di iniziare.

## Cosa non è automatico

- **Cfr.**, **Id.** ed **Ead.** si scrivono a mano in Word (procedura nelle regole di utilizzo).
- La **bibliografia ripartita per tipologia** (letteratura primaria, studi, altre opere) si fa a mano in Word.

## Segnalare un problema

Se trovi una discordanza tra l'output dello stile e le indicazioni del tuo relatore, apri una segnalazione nella sezione "Issues" indicando:

1. il tipo di fonte (libro, saggio, articolo, ecc.);
2. i campi compilati in Zotero (una schermata della scheda va benissimo);
3. l'output ottenuto e quello atteso, con il riferimento alla norma o all'esempio.

Non tutte le norme sono implementabili in CSL. Quando una segnalazione dipende da indicazioni diverse tra relatori, il file da modificare viene scelto caso per caso.

## Licenza

Il contenuto è distribuito con licenza Creative Commons Attribuzione - Non commerciale - Condividi allo stesso modo 4.0 Internazionale (CC BY-NC-SA 4.0). Vedi il file [LICENSE.md](LICENSE.md).

## Autrice

Maria Gualandris.
