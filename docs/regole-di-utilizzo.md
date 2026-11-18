# Regole di utilizzo: come compilare le voci in Zotero

Gli stili di questo repository leggono alcuni dati da campi particolari di Zotero, in modo che note e bibliografia escano corrette in Word senza ritocchi a mano. Questo documento elenca solo i casi particolari, quelli che è facile dimenticare. Per tutto il resto (autore, titolo, editore, anno) basta compilare i campi nel modo ovvio.

Le regole valgono per entrambi i file di stile, salvo dove indicato.

## Regole generali

- **Più autori o curatori.** Inseriscili in Zotero nello stesso ordine in cui devono comparire in nota e in bibliografia.
- **Il ruolo di una persona** (autore, curatore, traduttore) si cambia cliccando sull'etichetta "Autore" a sinistra del nome e scegliendo il ruolo dal menu.

## Traduttori e curatori

- **R1. Libro collettaneo senza autore.** I curatori vanno nel campo "Curatore"; il campo "Autore" resta vuoto.
- **R2. Libro con traduttore che è anche curatore.** Inserisci la stessa persona sia come "Traduttore" sia come "Curatore", scritta in modo identico carattere per carattere (nome, cognome, maiuscole). In nota esce "tr. it. a cura di ...".
- **R3. Libro con solo traduttore.** Compila il campo "Traduttore". In nota esce "tr. it. di ...".
- **R4. Libro con traduttore e curatore diverso dal traduttore.** Il traduttore va nel campo "Traduttore"; il curatore va nel campo "Series Editor", non in "Curatore". Esce "tr. it. di M. Bertani" prima del titolo e "a cura di F. Gros" dopo. Se per errore il curatore diverso viene messo in "Curatore", il suo nome esce prima del titolo: è un errore visibile, da correggere spostandolo in "Series Editor".

## Dati dell'edizione

- **R5. Luogo di edizione.** Scrivi nel campo esattamente come deve uscire, comprese le città multiple con trattino breve preceduto e seguito da spazio: `Roma - Bari`, `London - New York`, `Englewood Cliffs (N.J.)`. Se il tuo relatore vuole il trattino senza spazi, scrivilo così nel campo. Lo stile non modifica il testo.
- **R6. Edizione.** Nel campo "Edizione" scrivi solo il numero (`5`): esce in apice dopo l'anno. Se scrivi "5a ed." o altro testo, esce tutto in apice. Se si tratta della prima edizione, lascia il campo vuoto. Vale per libri e sezioni di libro; gli articoli non hanno il campo.
- **R7. In corso di stampa.** Nel campo "Extra" scrivi la riga `status: in corso di stampa` (il testo dopo i due punti è irrilevante, basta che la riga ci sia). Gli altri campi (editore, luogo, data) possono essere compilati o vuoti: lo stile stampa solo "in corso di stampa". Vale per libri, saggi e articoli.
- **R8. Opera in più volumi.** Nel campo "Numero di volumi" scrivi solo il numero (`6`). Nel campo "Volume" scrivi solo il numero arabo del volume citato (`5`): esce in numero romano ("V"). Se il volume ha un titolo, scrivilo nel campo "Extra" su una riga `volume-title: L'Ottocento`. Vale per libri, sezioni di libro e atti.
- **R9. Campo "Pagine".** Compilalo sempre con gli estremi completi di saggi, articoli e atti (`218-226`), senza "p." o "pp.". Serve sia nelle note sia in bibliografia. Non confonderlo con "# di Pagine" della scheda "Libro".

## Opere tradotte

- **R10. Traduzione con originale citato per esteso.**
  - "Titolo", "Editore", "Luogo di edizione", "Data", "Edizione": i dati della traduzione italiana.
  - "Editore originale": l'editore dell'originale (per esempio `J. Vrin`).
  - "Luogo originale": il luogo dell'originale (per esempio `Paris`).
  - "Data originale": solo l'anno (per esempio `1949`).
  - "Extra": una riga `original-title: En découvrant l'existence avec Husserl et Heidegger`, senza corsivo e senza caporali. La riga deve avere esattamente questa forma: nome della variabile in minuscolo, due punti, spazio, testo.
  - Per indicare l'anno della prima pubblicazione della traduzione italiana, scrivi in "Extra" una riga `event-date: 1967` (solo l'anno). Se coincide con l'anno del campo "Data", non scrivere la riga.
- **R11. Traduzione con solo l'anno dell'originale.** Compila solo "Data originale". Non scrivere `original-title` in "Extra": con quella riga la nota esce nella forma completa dell'R10 e l'anno non compare tra parentesi dopo il titolo. Per i libri tradotti compila sempre almeno "Data originale": senza `original-title` né "Data originale" non esce nessun anno dell'originale.

## Atti di convegno

- **R12. Atto di convegno.**
  - "Titolo": titolo del saggio. "Autore": autori del saggio. "Curatore": curatore degli atti.
  - "Titolo degli atti": titolo del volume (esce in corsivo).
  - "Nome del convegno": solo la dicitura che deve stare tra i caporali, compresi luogo e data, scritta come nell'esempio `Atti della Tavola rotonda, Roma 16 marzo 1996` (non scrivere le virgolette caporali). Se la dicitura costituisce essa stessa il titolo ("Atti del..."), scrivila in "Titolo degli atti" e lascia vuoto "Nome del convegno".
  - "Editore", "Luogo di edizione", "Data" (anno): i dati dell'edizione degli atti.
  - "Pagine": gli estremi del saggio (per esempio `89-104`).
  - "Luogo dell'evento": lascia vuoto.

## Fonti cartacee e fonti online

- **R13. Fonti da non indicare come web.** Lo stile stampa URL e data di consultazione ogni volta che il campo "URL" è compilato. Per ogni fonte da citare come cartacea (articolo di rivista, saggio, libro, voce di enciclopedia cartacea) svuota "URL" e "Consultato", anche se Zotero li ha compilati da solo al salvataggio (il connettore del browser lo fa per quasi tutti gli articoli: conviene fare la pulizia subito dopo l'importazione). Per non perdere il link, spostalo in "Extra" su una riga a parte (`link: https://...`) o in una nota allegata.
  - Controllo finale prima della consegna: in Zotero, "Ricerca avanzata", condizione sul campo "URL" con operatore "contiene" e valore `http`. Il risultato elenca tutte le fonti che usciranno come web.
- **R14. Fonti da indicare come web** (voci della Stanford Encyclopedia, articoli consultati solo online, pagine web). Compila sia "URL" sia "Consultato" (esce come "3 ottobre 2026"). Per la Stanford: tipo "Voce di enciclopedia", "Titolo dell'enciclopedia" `Stanford Encyclopedia of Philosophy`, "Data" con l'anno della versione citata.
- **R15. Annata e fascicolo degli articoli.** "Volume": solo numero arabo (`105`, esce "CV"). "Fascicolo": numero arabo. "Pagine": estremi completi (`218-226`). Per le fonti web: "Fascicolo" con il numero (`64`) e "Volume" vuoto, perché nel ramo web non è usato.

## Da fare a mano in Word

- **R16. Titolo breve.** Compila il campo "Titolo breve" solo per i titoli con sottotitolo che vuoi abbreviare nelle note successive; altrimenti nelle note successive esce il titolo intero.
- **R17. "Cfr.".** Scrivilo a mano in Word, prima del blocco Zotero (che appare evidenziato in grigio chiaro).
- **R18. Id./Ead. e bibliografia divisa in sezioni.** Questi elementi non sono gestiti dallo stile e vanno inseriti a mano in Word come ultima correzione, dopo aver selezionato "Unlink citations" (da quel momento il documento non è più collegato a Zotero, quindi fallo solo a lavoro finito).
  - **Id./Ead.**: sostituiscono il nome dell'autore quando due opere dello stesso autore compaiono nella stessa nota o in note consecutive.
  - **Bibliografia in sezioni**: se il relatore la vuole ripartita (per esempio opere dell'autore studiato, altri classici, studi, altre opere citate), crea le sezioni e sposta a mano le voci.
  - Con il file `ucsc-filosofia-maiuscoletto.csl`, anche Id./Ead. vanno scritti in maiuscoletto.
