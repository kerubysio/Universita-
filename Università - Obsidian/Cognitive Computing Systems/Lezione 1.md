MATERIA: [[Cognitive Computing Systems (6 CFU)]]
DATA: 13/03/2026

---

![[Pasted image 20260401204112.png|690]]
![[Pasted image 20260401204420.png]]

Vogliamo capire se la sagoma è un sopravvissuto a cui mandare dei soccorsi oppure no.
In questo caso si parla di "Problema cognitivo", perchè bisogna prendere delle decisioni sotto incertezza assumendosi le responsabilità delle scelte intraprese.

![[Pasted image 20260401205102.png]]

![[Pasted image 20260401205348.png]]
Un **Cognitive Computing System (CCS)** è un sistema di intelligenza artificiale progettato per simulare i processi di pensiero umani nel risolvere problemi complessi. A differenza dei software tradizionali, un CCS non si limita a eseguire istruzioni rigide, ma è in grado di **integrare dati provenienti da fonti diverse**, ragionare anche in situazioni di **incertezza** e imparare costantemente dall'esperienza per adattarsi a nuovi scenari. La sua particolarità risiede nella capacità di interagire in modo naturale con l'uomo e di saper **giustificare le proprie decisioni (explainability)**, rendendo il processo tecnologico più trasparente e collaborativo.
Una differenza fondamentale tra la pipeline ML e un sistema CCS sta proprio nel fatto che il primo agisce in maniera black box, mentre il secondo è sempre capace di spiegare i ragionamenti dietro alle proprie scelte.

![[Pasted image 20260402123659.png]]
Un'**Architettura Cognitiva Completa** rappresenta il framework strutturale di un CCS, organizzato come un ciclo continuo che trasforma i dati grezzi in azioni consapevoli. Il processo inizia con il **Sensing** e la **Perception** per acquisire e interpretare stimoli esterni, che vengono poi convertiti in una **Representation** (simbolica o sub-simbolica) del mondo. Su questa base, il sistema applica il **Reasoning**per valutare opzioni e il **Learning** per migliorare le prestazioni future. Il ciclo culmina nella **Decision**, ovvero la scelta dell'azione finale, il tutto mediato da un **Trust Layer**, un livello critico che garantisce l'affidabilità, l'etica e la trasparenza (explainability) dell'intero processo decisionale.

![[Pasted image 20260402123923.png]]
Il **Modello Bayesiano della Cognizione** propone che l'intelligenza funzioni come un meccanismo di **inferenza probabilistica** anziché come un semplice classificatore rigido. Secondo questa visione, la cognizione è un processo dinamico di aggiornamento delle conoscenze: il sistema parte da convinzioni preesistenti (**prior**), analizza nuovi dati o prove (**evidenze**) e integra queste informazioni per ottenere una visione aggiornata della realtà (**posterior**). In sostanza, il modello descrive la mente come una macchina statistica che impara e riduce l'incertezza attraverso il costante raffinamento delle probabilità basato sull'esperienza.

![[Pasted image 20260402124123.png]]
Il **Modello Bayesiano** ridefinisce la cognizione non come una classificazione statica (assegnazione di etichette), ma come un **aggiornamento continuo di credenze** espresse in termini probabilistici. In questo paradigma, l'incertezza non è un errore da eliminare, ma una variabile gestita esplicitamente: il sistema modula la propria fiducia in un'ipotesi man mano che riceve nuove informazioni. Questo approccio costituisce il fondamento dei sistemi cognitivi moderni, poiché permette loro di operare in ambienti reali complessi dove i dati sono spesso ambigui o incompleti, garantendo una flessibilità decisionale simile a quella umana.

![[Pasted image 20260402124224.png]]
Il **Teorema di Bayes** fornisce la base matematica per il ragionamento sotto incertezza nei sistemi cognitivi, permettendo di calcolare la probabilità di un'ipotesi ($H$) alla luce di un nuovo dato osservato ($D$). La formula

$$P(H|D) = \frac{P(D|H)P(H)}{P(D)}$$

esprime come la credenza aggiornata (**Posterior**) derivi dal prodotto tra la probabilità iniziale (**Prior**) e la verosimiglianza del dato osservato rispetto all'ipotesi (**Likelihood**), normalizzato per la probabilità totale del dato stesso. Questo meccanismo di **aggiornamento delle credenze** trasforma il calcolo statistico in un vero e proprio processo di apprendimento continuo, dove ogni nuova evidenza raffina o corregge la comprensione del mondo da parte del sistema.
