# 🛴 SmartMove - Sistema di Mobilità Sostenibile

## 📌 Descrizione del Progetto

SmartMove è una piattaforma web progettata per la gestione di servizi di mobilità sostenibile urbana e universitaria. L'applicazione consente agli utenti di registrarsi, effettuare il login, visualizzare i mezzi disponibili, avviare e terminare corse, effettuare pagamenti e segnalare eventuali guasti ai veicoli.

Il sistema è stato sviluppato come progetto didattico utilizzando tecnologie web moderne e un database cloud basato su Supabase.

---

## 🎯 Obiettivi del Progetto

L'obiettivo principale è simulare un servizio di sharing mobility simile a quelli utilizzati nelle smart cities, permettendo di:

* Ridurre l'utilizzo di veicoli privati.
* Favorire la mobilità sostenibile.
* Monitorare le corse effettuate dagli utenti.
* Gestire segnalazioni di manutenzione.
* Analizzare dati e statistiche tramite un pannello amministratore.

---

## ⚙️ Tecnologie Utilizzate

### Frontend

* HTML5
* CSS3
* JavaScript (Vanilla JS)

### Backend e Database

* Supabase
* PostgreSQL

### Librerie Esterne

* Supabase JavaScript SDK
* Leaflet.js
* OpenStreetMap

### Repository

* GitHub

---

## 🗄️ Struttura del Database

Il database è ospitato su Supabase e comprende le seguenti tabelle principali:

### Utenti

Contiene i dati degli utenti registrati.

| Campo              | Tipo      |
| ------------------ | --------- |
| id                 | UUID      |
| nome               | VARCHAR   |
| email              | VARCHAR   |
| data_registrazione | TIMESTAMP |

---

### Corse

Memorizza tutte le corse effettuate dagli utenti.

| Campo           | Tipo      |
| --------------- | --------- |
| id              | SERIAL    |
| id_utente       | UUID      |
| id_mezzo        | VARCHAR   |
| data_ora        | TIMESTAMP |
| durata_minuti   | INTEGER   |
| costo           | NUMERIC   |
| co2_risparmiata | NUMERIC   |

---

### Manutenzione

Gestisce le segnalazioni di guasti e manutenzione.

| Campo          | Tipo      |
| -------------- | --------- |
| id             | SERIAL    |
| id_mezzo       | VARCHAR   |
| componente     | VARCHAR   |
| descrizione    | TEXT      |
| stato          | VARCHAR   |
| data_creazione | TIMESTAMP |

---

### Pagamenti

Archivia i pagamenti effettuati dagli utenti.

| Campo          | Tipo      |
| -------------- | --------- |
| id             | SERIAL    |
| importo        | NUMERIC   |
| metodo         | VARCHAR   |
| stato          | VARCHAR   |
| data_pagamento | TIMESTAMP |

---

## 📄 Pagine del Progetto

### Login

Permette agli utenti registrati di accedere al sistema tramite email e password.

**File:** `login.html`

---

### Registrazione

Consente la creazione di un nuovo account e il salvataggio dei dati nel database Supabase.

**File:** `register.html`

---

### Dashboard Principale

Visualizza:

* Mappa dei mezzi disponibili.
* Wallet utente.
* Collegamenti rapidi.
* Veicoli disponibili nelle vicinanze.

**File:** `index.html`

---

### Storico Corse

Mostra l'elenco delle corse effettuate dagli utenti.

**File:** `history.html`

---

### Sessione di Guida

Simula una corsa attiva mostrando:

* Tempo trascorso.
* Velocità.
* Costo accumulato.
* Risparmio di CO₂.

**File:** `unlock.html`

---

### Segnalazione Guasti

Permette agli utenti di segnalare problemi ai veicoli.

**File:** `report.html`

---

### Pagamenti

Gestisce lo storico e la registrazione dei pagamenti.

**File:** `pagamenti.html`

---

### Pannello Amministratore

Permette di monitorare:

* Ticket di manutenzione.
* Stato della flotta.
* Dati aggregati del sistema.

**File:** `admin.html`

---

## 🌍 Funzionalità Implementate

✅ Registrazione utenti

✅ Login con Supabase Authentication

✅ Gestione sessioni utente

✅ Visualizzazione mezzi su mappa interattiva

✅ Simulazione corsa

✅ Salvataggio corse nel database

✅ Storico pagamenti

✅ Segnalazione guasti

✅ Dashboard amministrativa

✅ Database cloud PostgreSQL

---

## 🚀 Possibili Sviluppi Futuri

* Integrazione con sistemi di pagamento reali (Stripe, PayPal).
* Geolocalizzazione GPS in tempo reale.
* QR Code per sblocco veicoli.
* Notifiche push.
* Applicazione mobile Android/iOS.
* Analisi avanzata dei dati tramite dashboard statistiche.

---

## 👨‍💻 Autore

**Alessandro Costa**

Progetto sviluppato per finalità didattiche nell'ambito del corso:

**IS-MM-ICD 2025/2026**

Università degli Studi di Bari "Aldo Moro"

---

## 📜 Licenza

Questo progetto è stato realizzato esclusivamente per scopi didattici e dimostrativi.
