# Guida V6.6 - Mittenti autorizzati

Questa versione modifica il modulo **Scarica Mail**.

## Regola operativa
Scarica solo email e allegati provenienti da:

- elibetty731@gmail.com
- Valentinaboratto82@gmail.com
- stefano.faraone@eurofintechsrl.it
- praticheBS@proton.me
- sergio.pedolazzi@katudi.it
- paolo.baldinelli@katudi.it
- pratiche@katudi.it
- niccolo.sovico@ener2crowd.com

## Uso
1. Avvia la web app Streamlit.
2. Vai su **Scarica Mail**.
3. Inserisci server IMAP, account e password/app password.
4. Lascia vuoto il campo **Mittente specifico autorizzato** per scaricare tutti gli 8 mittenti.
5. Inserisci un mittente specifico solo se vuoi scaricare uno degli 8 indirizzi.
6. Premi **Scarica Mail** oppure **Scarica tutte le mail nuove**.

## Effetto
- Le email non provenienti dagli 8 mittenti vengono ignorate.
- I mittenti vengono rilevati automaticamente.
- I clienti vengono creati automaticamente in anagrafica quando riconosciuti da mail/allegati.
- Gli allegati vengono salvati e collegati alla scheda azienda.
