# VOID - Scripts

Raccolta di alcuni script utili per void linux

---

**Release: 20230125.1145**

---

## Scripts

**service**

Bash scripts che simula il comando service <systemd service name> <action> adattato a runit.

Attenzione per la natura di runit quando si eseguirà un enable/disable sarà automaticamente avviato/arrestato il servizio.

Eseguire il comando senza parametri mostrerà un messaggio con tutte le opzioni e i comandi disponibili.


**xbps-vur**

xbps Void User Repository è semplicemente un wrapper per i comandi comuni che si inviano a xbps-src.

I comandi supportati sono:

 - aggiorna: esegue un check dei pacchetti compilati per verificare che vi sia un aggiornamento
 - cerca: ricerca un pacchetto nel repository
 - rimuovi: rimuove un pacchetto installato e cancella eventuali pacchetti compilati dal respository
 - installa: compila e installa un pacchetto dal respository

Se invocato usando un comando diverso dai 4 sopra elencati il comando sarà inviato direttamente a xbps-src.

Lo script utilizza /opt/void-packages come path per la gestione di xbps-src e dell'environment di compilazione.
