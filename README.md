# LEXIA Pro · prototipo cliccabile (Allegato C)

Prototipo dell'interfaccia di LEXIA Pro per il Project Work MEIA.

## File
- `index.html`: prototipo principale (versione Organic). Apre la panoramica, le varianti 1a–1d e il prototipo navigabile: lettura CAA (touch, dwell, scansione a singolo switch), marcatura docente, risultati con grafico dell'andamento, impostazioni, archivio letture, storia in CAA "Biancaneve", classi e alunni con codici anonimi, guida LEXIA.
- `broadsheet.html`: la stessa interfaccia nello stile Broadsheet (versione precedente, senza archivio e classi).
- `assets/caa/`: pittogrammi ARASAAC usati nelle tessere.
- `assets/biancaneve/`: illustrazioni e simboli della storia "Biancaneve" (dal documento biancaneve.docx).
- `src/`: sorgenti modificabili dei due prototipi.

`index.html` e `broadsheet.html` sono autosufficienti, ma `index.html` carica i pittogrammi dalla cartella `assets/`: tenerla accanto al file.

## Pubblicazione con GitHub Pages
Settings → Pages → Source: *Deploy from a branch* → branch `main`, cartella `/ (root)`.
Il prototipo sarà su `https://hope75-ui.github.io/project-work-meia/`.

## Note di progetto (da riportare nell'Allegato C)
- Nessun modello predittivo: WPM, LPM e accuratezza sono formule esplicite; la tendenza nel grafico è una regressione lineare sulle sessioni incluse dal docente.
- La voce dell'alunno non viene registrata né analizzata. La correttezza della lettura è marcata dal docente.
- Classi, codici alunno e testi aggiunti sono salvati nel `localStorage` del dispositivo. I nomi usati per generare i codici restano solo in memoria e non vengono salvati: si tratta di pseudonimizzazione (art. 4, n. 5 GDPR), perché la chiave di corrispondenza consente di risalire all'alunno.
- Le sessioni precedenti mostrate nel grafico sono dati di esempio.
- Testi dell'archivio: pubblico dominio (Collodi, De Amicis, Pascoli) o scritti dal docente.

## Crediti e licenze
- Pittogrammi: Sergio Palao · Origine: ARASAAC (arasaac.org) · Licenza: CC BY-NC-SA · Proprietà: Governo di Aragona (Spagna).
- I simboli della storia "Biancaneve" sembrano PCS (Boardmaker), con licenza proprietaria: prima di una pubblicazione aperta verificare la licenza della scuola o sostituirli con pittogrammi ARASAAC.
