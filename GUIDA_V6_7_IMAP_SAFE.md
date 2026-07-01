# FinancePlus 360 TOP v6.7 - IMAP SAFE

## Perché questa versione

La versione corregge il problema IMAP:

```text
[OVERQUOTA] Account exceeded command or bandwidth limits
```

Questo messaggio viene restituito dal provider mail quando la casella supera temporaneamente i limiti di banda o comandi IMAP.

## Cosa cambia

- Scarico solo dagli 8 mittenti autorizzati.
- Prima lettura leggera degli header.
- Salto automatico delle email già archiviate.
- Limite configurabile: massimo mail per click.
- Anti-duplicato allegati tramite hash MD5.
- Clienti creati automaticamente solo se riconosciuti con sufficiente certezza.
- Documenti non abbinati salvati in `Temporanea_Da_Abbinare`.

## Uso consigliato

1. Impostare massimo 10 o 20 mail per click.
2. Usare intervalli date piccoli, per esempio 1-7 giorni.
3. Non cliccare ripetutamente se compare OVERQUOTA.
4. Attendere il reset del provider e riprovare.
