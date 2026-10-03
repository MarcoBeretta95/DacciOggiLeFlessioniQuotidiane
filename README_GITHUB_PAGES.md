# Dacci oggi le flessioni quotidiane — GitHub Pages + Firebase

## 1. File da pubblicare

Carica `index.html` nel repository GitHub. GitHub Pages pubblicherà direttamente questo file.

## 2. Firebase

Il file è già configurato per il progetto Firebase:
`dacci-oggi-le-flessioni`

Il database usato è Cloud Firestore.

## 3. Attivare Firestore

Nel Firebase Console:

1. Apri il progetto `dacci-oggi-le-flessioni`.
2. Vai in **Build → Firestore Database**.
3. Crea il database.
4. Seleziona la modalità/regione richiesta da Firebase.
5. In **Rules**, per il primo test, puoi usare il contenuto di `firestore.rules`.

ATTENZIONE: queste regole permettono a chiunque conosca l'app di leggere e modificare i dati. Sono adatte solo per un primo test della challenge. Prima di usare l'app con dati che vuoi proteggere, bisogna aggiungere Firebase Authentication e regole basate sull'utente/gruppo.

## 4. GitHub Pages

Nel repository GitHub:

1. Vai in **Settings → Pages**.
2. In **Build and deployment** scegli **Deploy from a branch**.
3. Branch: `main`.
4. Folder: `/ (root)`.
5. Salva.

Dopo la pubblicazione, GitHub mostrerà l'indirizzo del sito.

## 5. Funzioni disponibili

- Flessioni, squat, lunges, pull up/chin up, plank, crunches e leg raises.
- Obiettivi giornalieri predefiniti e scelta della cadenza giornaliera o settimanale già quando si aggiunge una persona; gli obiettivi si possono personalizzare nella scheda “Persone & obiettivi” e i target mensili e settimanali si aggiornano in base agli obiettivi correnti.
- Target mensili calcolati automaticamente in base agli obiettivi individuali giornalieri o settimanali.
- Il plank viene registrato e conteggiato in minuti; gli altri esercizi in ripetizioni.
- Inserimento attività con data scelta manualmente, anche retroattiva.
- Storico condiviso.
- Dashboard mensile.
- Progresso settimanale.
- Dati condivisi tramite Firestore tra browser e dispositivi diversi.
