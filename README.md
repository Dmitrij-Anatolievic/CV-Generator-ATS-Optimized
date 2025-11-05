# CV Generator Pro (Ottimizzato ATS)

> Un'applicazione desktop "meta" (Python/PyQt) che ho costruito per risolvere il mio stesso problema: generare CV professionali ottimizzati per "hackerare" i sistemi di Applicant Tracking System (ATS) dei recruiter.

---

## 💡 Il Problema (Perché questo progetto?)

Come discusso nella mia ricerca di lavoro, il 90% delle candidature fallisce prima ancora di raggiungere un umano. Il motivo è che i CV non sono formattati per i software **ATS**, che scartano automaticamente i documenti in base a parole chiave e layout.

Creare un CV a mano è un "lavoro nel lavoro":
* **Fallimento ATS:** I CV creativi (fatti con Word o Canva) non possono essere letti dagli scanner.
* **Inefficienza:** È frustrante dover creare 30.000 versioni diverse di un CV.
* **Mancanza di Coerenza:** Gestire più versioni porta a errori e formattazioni diverse.

## 🚀 La Soluzione (Cosa fa il progetto?)

Ho sviluppato **CV Generator Pro**, l'applicazione che sto usando per creare i miei stessi documenti.
È un tool desktop che risolve tutti questi problemi:
1.  **Anti-ATS:** Genera file HTML e PDF con un layout pulito a colonna singola, usando solo font "ATS-safe" (Arial, Calibri) e tag semantici.
Il codice include anche una funzione `test_ats_compatibility` per valutare il punteggio del CV.
2.  **Database CV Sicuro:** Salva ogni CV in un database SQLite locale, con **checksum SHA-256** per l'integrità dei dati, **versioning** e un **audit log** completo per tracciare ogni modifica.
3.  **Alta Professionalità:** Include 50 temi professionali diversi (divisi per categorie: Classico, Moderno, Elegante...) e un'anteprima in tempo reale (QWebEngineView).

## 🎥 Demo Video

<img width="1916" height="991" alt="image" src="https://github.com/user-attachments/assets/40c8dc6f-e2e1-421d-8e26-29270acf93fd" />


**[Guarda la Demo su YouTube] (link-demo-youtube)**

## 🛠️ Tecnologie Utilizzate (Skills Dimostrate)

* **Linguaggio:** Python
* **GUI:** PyQt6 (interfaccia complessa a schede, dialoghi modali, QWebEngineView per l'anteprima)
* **Database:** SQLite (con gestione avanzata: `hashlib` per checksum SHA-256, versioning, audit log)
* **Reporting PDF/HTML:** Generazione di file HTML ottimizzati e PDF tramite `pdfkit`.
* **Gestione Temi:** Sistema modulare per la gestione di 50 temi.
* **Gestione Immagini:** `Pillow` (per ottimizzare e applicare crop circolari alle foto profilo).

## 🔑 Caratteristiche Principali

* **Generazione Ottimizzata ATS:** La funzione chiave. Produce CV progettati per essere letti correttamente dagli scanner dei recruiter.
* **Database CV Locale:** Un database sicuro per salvare, caricare e gestire diverse versioni dei tuoi CV.
* **Checksum e Integrità:** Ogni salvataggio è verificato con un hash SHA-256 per prevenire la corruzione dei dati.
* **50 Temi:** Vasta libreria di temi professionali tra cui scegliere.
* **Esportazione PDF e HTML:** Esporta in formati universalmente accettati.
* **Interfaccia Completa:** GUI intuitiva per gestire ogni sezione: Dati Personali, Esperienze, Istruzione, Competenze (Tecniche/Trasversali), Lingue e Info Aggiuntive.

## 📜 Licenza e Proprietà

**© 2025 Dmitrij Musella - Tutti i diritti riservati.**

Il codice sorgente di questo progetto è **privato** e non può essere copiato, modificato o distribuito senza esplicito consenso scritto da parte dell'autore.

Le demo video sono fornite a solo scopo dimostrativo del portfolio.
