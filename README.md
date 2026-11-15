# [SOSTIENI IL PROGETTO TOUGHCHAT!](https://github.com/sponsors/marcodadamo/sponsorships?sponsor=marcodadamo&tier_id=682579&preview=false) 

# 💬 ToughChat

**ToughChat** è un'applicazione Android di messaggistica istantanea progettata con un approccio *privacy-first*, crittografia end-to-end (E2EE) avanzata, strumenti di ispezione crittografica in tempo reale e un assistente di intelligenza artificiale integrato.

---

## 🛡️ Architettura di Sicurezza e Crittografia

* **Crittografia End-to-End (E2EE):** I messaggi transitano sui server esclusivamente in formato cifrato inaccessibile. La decifratura in chiaro avviene unicamente nella memoria locale del dispositivo prima della visualizzazione.
* **Gestione Identità Crittografica:**
  * Generazione e visualizzazione del **Fingerprint SHA-256** univoco dell'utente.
  * Esportazione e consultazione della **Chiave Pubblica Completa** (architettura ibrida AES/RSA).
* **Modalità Ispettore E2EE:** Strumento di debug e trasparenza integrato che permette di visualizzare i *byte cifrati grezzi* e il *vettore di inizializzazione (IV)* direttamente all'interno delle bolle della chat.
* **Messaggi Effimeri (Auto-distruzione):** Timer configurabile per l'eliminazione automatica dei messaggi dopo la lettura (`Disattivato`, `10s`, `30s`, `5m`, `1h`).

---

## 🤖 Assistente AI Integrato: ToughBot (Gemini)

ToughChat integra **ToughBot**, un assistente AI basato su **Gemini** configurabile su tre profili specializzati per la sicurezza informatica:

1. **Esperto Crittografia & E2EE:** Analizza protocolli, chiavi AES/RSA e verifica l'integrità crittografica delle comunicazioni.
2. **Consulente Privacy & Diritti:** Fornisce supporto e linee guida su riservatezza delle comunicazioni e normative sulla privacy.
3. **Cyber Intelligence (Argon):** Motore di ragionamento avanzato dedicato all'analisi di vettori di attacco e tecniche di steganografia.

---

## ✨ Funzionalità Principali

### 📱 Gestione Contatti & Discovery
* **Verifica Diretta per Email:** Ricerca istantanea di un indirizzo email per verificare la registrazione a ToughChat e lo stato di attivazione sul dispositivo del destinatario.
* **Scansione Rubrica Locale:** Controllo automatizzato dei contatti salvati sul telefono con statistiche su email rilevate, utenti registrati e app attiva.

### 🔔 Sistema di Notifiche ad Alta Affidabilità (`ToughChatSyncService`)
* **Servizio in Background Persistente:** Il demone `ToughChatSyncService` garantisce la ricezione istantanea dei messaggi anche ad app chiusa o rimossa dalla memoria recente.
* **Gestione Doze Mode:** Collegamento diretto alle impostazioni di sistema Android per escludere l'app dalle restrizioni di ottimizzazione della batteria.
* **Notifiche a Schermo Bloccato:** Risveglio automatico dello schermo con consegna ad alta priorità e visibilità pubblica sicura (decifratura locale *on-the-fly*).
* **Diagnostica Integrata:** Pulsante per l'invio di una notifica di test cifrata E2EE per verificare il corretto funzionamento della tendina e della schermata di blocco.

### 📝 Spazio di Lavoro: Canvas ToughChat & Profilo
* **Canvas ToughChat (HTML Editor):** Spazio personale sincronizzato per la redazione di appunti e documenti strutturati tramite codice HTML puro, con visualizzatore del codice sorgente integrato.
* **Personalizzazione Interfaccia:** Supporto nativo per doppia modalità visiva:
  * *Bianco (Luminoso)* con accenti azzurri ToughChat.
  * *Scuro (Cyber Dark)* ad alto contrasto per l'uso notturno.
* **Profilo Social:** Sezione dedicata alla gestione dell'avatar, ID utente univoco e collegamento rapido al profilo social.

---

## 🧭 Struttura dell'Interfaccia (Navigation)

L'applicazione è organizzata su una barra di navigazione inferiore a 4 schede principali:
1. **Chat:** Elenco delle conversazioni E2EE e barra di ricerca globale.
2. **Contatti:** Rubrica sincronizzata, filtri rapidi (*Tutti*, *Con ToughChat*, *Con Email*) e strumento di verifica diretta.
3. **Notifiche:** Centro di diagnostica `ToughChatSyncService`, test di ricezione e gestione risparmio energetico.
4. **Impostazioni:** Gestione profilo, accesso a *Canvas ToughChat*, selettore tema, chiavi crittografiche, timer messaggi effimeri e configurazione di *ToughBot*.

---

## 👨‍💻 Autore

Sviluppato da **Marco D'Adamo**

