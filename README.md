# FinancePlus 360 TOP v6.7 IMAP SAFE - MITTENTI AUTORIZZATI

Correzione specifica:
- il campo amministratore non deve più valorizzarsi con testi errati come "Data di"
- rafforzata l'estrazione di nome e cognome del legale rappresentante / amministratore
- la correzione automatica riesamina anche i record che hanno valori amministratore errati

## Dopo aggiornamento
1. aggiorna i file su GitHub / Streamlit
2. riavvia l'app
3. vai in Impostazioni > Correzione dati
4. clicca Correggi automaticamente anagrafiche esistenti
5. se il testo estratto non contiene davvero il nome, usa la modifica manuale in Scheda Azienda > Anagrafica oppure reimporta la visura


## Modifica V6.6 - Scarico mail filtrato per mittenti autorizzati

Il modulo **Scarica Mail** ora scarica esclusivamente email e allegati provenienti dai seguenti indirizzi:

- elibetty731@gmail.com
- Valentinaboratto82@gmail.com
- stefano.faraone@eurofintechsrl.it
- praticheBS@proton.me
- sergio.pedolazzi@katudi.it
- paolo.baldinelli@katudi.it
- pratiche@katudi.it
- niccolo.sovico@ener2crowd.com

Tutte le altre email vengono ignorate automaticamente, anche se contengono allegati.

La creazione automatica del cliente in anagrafica resta attiva: quando il sistema riconosce un'azienda da oggetto, corpo email, allegati, P.IVA, codice fiscale o PEC, crea/aggiorna l'anagrafica e abbina i documenti. I documenti non abbinabili restano in gestione come cliente automatico/da verificare.


## Aggiornamento v6.7 - IMAP SAFE

Questa versione riduce il rischio di errore `OVERQUOTA` IMAP:

- scarica solo dagli 8 mittenti autorizzati;
- legge prima solo gli header delle email;
- salta le email già archiviate tramite Message-ID;
- consente di impostare un limite massimo di mail per click;
- evita duplicati allegati tramite hash MD5;
- manda in `Temporanea_Da_Abbinare` i documenti non riconosciuti.

Se il provider restituisce ancora `OVERQUOTA`, non è un errore del programma: la casella ha superato il limite temporaneo di banda/comandi IMAP. Attendere il reset e riprovare con 10-20 email per click.
