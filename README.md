# Basi di Dati – Database per una piattaforma di live streaming

## Introduzione

Progetto del corso di **Basi di Dati** (Laurea Triennale in Informatica, UniTo).
Progettazione e realizzazione di una base di dati per un servizio di **live streaming** liberamente ispirato a Twitch: utenti spettatori e streamer, canali, live, video e clip, chat, follower e abbonamenti, portafoglio di bit e donazioni, calendario delle live. Il progetto è stato sviluppato in gruppo per il corso di TLN, insieme a un collaboratore.

## Tecnologie usate

* **SQL** (DDL, DML, viste e query)
* Schemi **E-R** per la progettazione concettuale e logica

## Riassunto delle parti

### Parte 1 – Progettazione concettuale

Analisi dei requisiti, glossario dei termini, raggruppamento dei requisiti in frasi omogenee e costruzione dello **schema E-R** con le business rules.

### Parte 2 – Progettazione logica

* **Tavola dei volumi** e **tavola delle operazioni** con le frequenze stimate
* **Ristrutturazione dello schema E-R**: analisi delle ridondanze (calcolo di accessi e spazio per decidere se tenere o eliminare attributi derivati, come il numero di spettatori, visualizzazioni, follower e abbonati), eliminazione delle generalizzazioni e degli attributi composti, scelta degli identificatori
* **Schema relazionale** con i vincoli di integrità

### Parte 3 – Implementazione

* **DDL**: creazione di tabelle, viste e vincoli (chiavi, `check`, `unique`, chiavi esterne con `on update` e `on delete`)
* **DML**: popolamento di tutte le tabelle con dati di prova
* **Query di prova**: numero di follower e di abbonati, visualizzazioni di clip e video, aggiornamento dei dati dello streamer e degli spettatori attuali per categoria, calcolo degli *affiliate* (500 minuti trasmessi, almeno 3 spettatori medi, almeno 50 follower) e classifica degli streamer più seguiti

