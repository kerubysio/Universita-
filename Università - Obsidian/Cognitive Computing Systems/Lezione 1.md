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

![[Pasted image 20260402124601.png]]
L'equazione **Cognizione = Stato di Credenze** esprime l'idea che un sistema cognitivo non abbia mai un accesso diretto e assoluto alla realtà oggettiva, ma operi esclusivamente attraverso **distribuzioni di probabilità**. In questo modello, il sistema osserva solo segnali rumorosi o parziali e deve **inferire lo stato più plausibile** del mondo esterno. Di conseguenza, ogni scelta non avviene sulla realtà stessa, ma in uno **spazio delle credenze** (_belief space_): il sistema prende decisioni basandosi sulla configurazione di probabilità che ritiene più verosimile in quel momento, accettando intrinsecamente il margine di incertezza tipico di ogni processo cognitivo avanzato.

![[Pasted image 20260402124736.png]]
L'**aggiornamento della credenza** è il cuore operativo del ciclo cognitivo, dove il valore calcolato come **Posterior** smette di essere un semplice risultato numerico e diventa il **nuovo stato cognitivo** del sistema. Attraverso la formula che combina la conoscenza pregressa (**Prior**) con la verosimiglianza dei nuovi dati (**Likelihood**) normalizzati rispetto all'**Evidenza**, il sistema evolve la propria percezione della realtà. Questo processo garantisce la continuità dell'apprendimento: ciò che era una conclusione in un determinato momento (il _posterior_ attuale) fungerà da punto di partenza (la _prior_ futura) per l'osservazione successiva, permettendo al sistema di affinare costantemente la propria interpretazione del mondo.

![[Pasted image 20260402124843.png]]
La **visualizzazione dell'aggiornamento bayesiano** mostra graficamente la relazione tra la verosimiglianza del dato osservato (**Likelihood**) e la nuova credenza generata (**Posterior**). La curva illustra come, all'aumentare della probabilità che un certo dato $D$ sia spiegato dall'ipotesi $H$, cresca proporzionalmente la fiducia del sistema in quell'ipotesi stessa. In un sistema cognitivo, questo grafico rappresenta la sensibilità del modello all'evidenza: una pendenza più o meno ripida indica quanto velocemente il sistema è disposto a cambiare idea o a consolidare la propria "certezza" in risposta a ciò che osserva nell'ambiente.

![[Pasted image 20260402125015.png]]
Un sistema intelligente produce credenze, non risposte.

![[Pasted image 20260402125146.png]]
Perchè è cruciale questo ragionamento ora?
Perchè quantifica l'incertezza.

La capacità di produrre **credenze probabilistiche** anziché risposte rigide è fondamentale nei sistemi **safety-critical** (come la guida autonoma o la diagnostica medica) perché permette di **quantificare l'incertezza**. In questi contesti, sapere quanto il sistema sia "insicuro" della propria percezione è vitale per supportare decisioni basate sull'**utilità attesa**, dove si bilanciano i rischi e i benefici di ogni azione. Questa trasparenza statistica costituisce la base per la **certificazione** e la costruzione della fiducia (_trust_): un sistema che ammette il proprio grado di dubbio è intrinsecamente più sicuro di uno che fornisce risposte binarie potenzialmente errate, permettendo interventi umani o procedure di sicurezza quando la fiducia nell'ipotesi scende sotto una soglia critica.

![[Pasted image 20260402125432.png]]
Il modello bayesiano è considerato un vero **modello di cognizione** perché non si limita a catalogare i dati, ma implementa una **dinamica epistemica**, ovvero una gestione attiva della conoscenza. A differenza della classificazione statica, questo approccio introduce l'**incertezza esplicita** come parte integrante del sistema, permettendo una **rappresentazione delle credenze** che evolve nel tempo. Attraverso l'**apprendimento incrementale** e la costante **revisione delle convinzioni** alla luce di nuove prove, il sistema simula il modo in cui una mente intelligente aggiorna la propria comprensione del mondo, rendendo il pensiero un processo fluido di adattamento continuo anziché una serie di risposte pre-programmate.

![[Pasted image 20260402125638.png]]
Il prof non ha detto molto su questa slide, non approfondire.

![[Pasted image 20260402125719.png]]

La differenza fondamentale tra il **Deep Learning (DL) classico** e la **Cognizione Bayesiana** risiede nella gestione della conoscenza interna. Il DL puro opera generalmente come una funzione matematica che mappa direttamente un input a un output (ad esempio, un'immagine alla sua etichetta), focalizzandosi sulla precisione del risultato finale.
Al contrario, la cognizione bayesiana mantiene uno **stato interno di credenze** espresso tramite **distribuzioni di probabilità** che vengono costantemente aggiornate.
Sebbene una rete neurale possa stimare una probabilità $P(H|D)$, essa spesso manca di un **modello probabilistico completo** ed esplicito; l'approccio bayesiano, invece, integra nativamente l'**incertezza**, permettendo al sistema non solo di dare una risposta, ma di "sapere di non sapere" e di motivare il proprio grado di fiducia in ogni specifica situazione.

![[Pasted image 20260402130026.png]]

L'affermazione **"Un sistema intelligente non produce risposte, produce credenze aggiornate"** rappresenta il superamento dell'AI come semplice calcolatore deterministico verso una **Explainable AI (XAI)** basata sulla fiducia. In questo paradigma, l'intelligenza non è definita dall'assenza di errore, ma dalla capacità di fornire una **giustificazione comprensibile** (credenza) del proprio output. Mentre un modello "black box" fornisce una risposta secca che può risultare inaffidabile o generare allucinazioni (risposte false ma convincenti), un sistema intelligente collabora con l'uomo contestualizzando le proprie conclusioni. Questo permette all'utente di identificare eventuali **bias** o limiti logici del modello, rendendo l'errore un evento gestibile e comprensibile invece di un fallimento inspiegabile del sistema.
Se l'errore è trasparente e comprensibile, l'IA non agisce come un oracolo sempre corretto, ma come un assistente.

![[Pasted image 20260402130337.png]]

"Perchè è cruciale avere sistemi con un approccio cognitivo moderno?"

![[Pasted image 20260402130504.png]]

L'**Architettura di un Sistema Cognitivo Moderno** è organizzata in cinque livelli gerarchici che trasformano i dati grezzi in decisioni affidabili.
Si parte dal **Data Layer** (sensori e streaming multimodale) e dal **Perceptual Layer**, dove tecnologie come CNN e LLM interpretano i segnali.
Il cuore del sistema è il **Cognitive Layer**, che utilizza Knowledge Graphs e Reti Bayesiane per il ragionamento simbolico e neurale (Hybrid AI).
Segue il **Decision Layer**, che pianifica le azioni tramite Reinforcement Learning e modelli MDP (lo vedremo più avanti).
Infine, il **Trust Layer** garantisce la sicurezza attraverso l'**Explainability** (SHAP, LIME), la robustezza agli attacchi e il rispetto dei vincoli etici, rendendo l'intero sistema trasparente e certificabile.

![[Pasted image 20260402130716.png]]

Facciamo un breve cenno a ciascuna di queste nelle prossime slides

![[Pasted image 20260402130857.png]]

La **Teoria dell'Utilità** rappresenta il passaggio dalla pura conoscenza all'azione: se Bayes risponde alla domanda "Cosa credo sia vero?", la decisione ottimale risponde a "**Cosa mi conviene fare?**". Formalmente, l'azione ottima $a^*$ è quella che massimizza l'utilità attesa, calcolata come la media pesata delle utilità di ogni possibile stato futuro rispetto alla loro probabilità: $a^* = \text{argmax}_a \sum P(s|a) U(s)$. Questo approccio è cruciale in ambiti come quello aerospaziale o nel _mission planning_, dove non si massimizza la semplice probabilità di successo, ma la **sopravvivenza** (safety > efficienza).
Attraverso il trade-off tra rischi e benefici e l'applicazione delle equazioni di Bellman, il sistema agisce come un co-pilot cognitivo capace di scegliere la rotta che garantisce il miglior equilibrio tra il raggiungimento dell'obiettivo e la mitigazione dei pericoli.

![[Pasted image 20260402174351.png]]
![[Pasted image 20260402174408.png]]
L'operatore **$\text{arg max}$** (abbreviazione di _argument of the maximum_) indica il valore dell'argomento $a$ per il quale la funzione raggiunge il suo valore massimo. Mentre il "max" di una funzione restituirebbe il valore dell'utilità più alta possibile, l'**$\text{arg max}$** restituisce l'**azione specifica** ($a^*$) che permette di ottenere quel risultato. In termini pratici, all'interno della formula della decisione ottimale, esso rappresenta il "motore di scelta" del sistema: dopo aver calcolato l'utilità attesa per ogni possibile azione disponibile, il sistema seleziona e mette in atto quella che garantisce il valore statistico migliore, trasformando il calcolo probabilistico in un comportamento concreto e razionale.

![[Pasted image 20260402174545.png]]

L'**interpretazione della decisione ottima** chiarisce che il sistema non sceglie l'azione semplicemente più probabile, ma quella che massimizza il valore atteso delle conseguenze. Nel calcolo dell'**utilità attesa**, la probabilità $P(s|a)$ rappresenta l'incertezza sul mondo, mentre $U(s)$ quantifica il valore (o il costo) di ciò che accadrebbe in quello stato.

![[Pasted image 20260402174722.png]]

L'esempio del drone da soccorso è emblematico: anche con una probabilità del **30%** di un falso positivo (un errore), l'utilità attesa di inviare la squadra resta elevata (**67**) perché il valore di salvare una vita (+100) sovrasta di gran lunga il costo del falso allarme (-10). Questo **criterio razionale** permette al sistema di agire in modo etico e sicuro, bilanciando matematicamente i rischi di un errore con i benefici di un successo critico.

![[Pasted image 20260402174755.png]]

![[Pasted image 20260402174817.png]]

![[Pasted image 20260402174846.png]]
La **differenza tra Machine Learning (ML) classico e decisione ottimale** segna l'evoluzione del sistema da un semplice strumento di previsione a un'entità con **decision authority**.
Mentre un classificatore standard punta unicamente a minimizzare l'errore medio (accuratezza statistica), la decisione ottimale mira a **massimizzare l'utilità attesa** (o minimizzare il costo atteso), tenendo conto dell'**asimmetria del rischio**. In contesti reali, non tutti gli errori hanno lo stesso peso: ignorare un ostacolo sulla strada è infinitamente più grave che frenare inutilmente.
Questo approccio permette al sistema di non essere solo "preciso", ma "saggio", poiché valuta le conseguenze delle proprie azioni in base al contesto e alla sicurezza, trasformando la pura _prediction_ in una scelta strategica e responsabile.

![[Pasted image 20260402175022.png]]

![[Pasted image 20260402175132.png]]

Questa slide illustra l'applicazione dell'**Utilità Attesa in uno scenario di emergenza** (guasto motore in volo), mettendo a confronto due strategie decisionali. Il grafico 3D mostra come l'**Utilità Attesa (asse Z)** vari in base alla **Probabilità di guasto (asse X)** e alla scala di valori assegnati alle conseguenze (**asse Y**). La linea blu rappresenta l'atterraggio immediato, che mantiene un'utilità stabile e sicura, mentre la linea arancione rappresenta il continuare il volo, la cui utilità crolla drasticamente all'aumentare della probabilità di guasto. Il punto in cui le due linee si incrociano definisce la **soglia decisionale**: oltre quel livello di incertezza, il sistema razionale "scatta" e impone l'atterraggio, dimostrando come la decisione non dipenda solo dal rischio calcolato, ma dal peso catastrofico assegnato a un possibile fallimento del motore.

![[Pasted image 20260402175252.png]]

