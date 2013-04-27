Color-Detector
==============

this system identifies the color of objects and try to divide them by that color


Salve a tutti,
grazie per aver scaricato questo software! Siete i migliori!

Questo progetto è stato realizzato da Davide Pasetto e Lorenzo Pedrotti  e colgo l'occassione per ringraziare chi ci ha sostenuto e aiutato nella realizzazione di  questo progetto che tra l'altro è stata la nostra tesina per la maturità, anno 2013.

Il software è di libero dominio e può essere copiato, modificato e ridistribuito liberamente.

Lo sketch utilizza librerie standard di Arduino, la libreria "servo.h" e la "EEPROM.h" quindi non dovrebbero esserci nella compilazione.

Il sistema permette di individuare il colore degli oggetti e grazie ad un motore passo-passo vengono separate tra i colori ROSSO; VERDE; BLU e NON CLASSIFICATO che come suggerisce il nome sta ad indicare che il colore non viene riconosciuto tra quelli predefiniti.

Il sistema utilizza vari integrati di contorno, alcuni essenziali al corretto funzionamento altri meno, per la rotazione del motore passo-passo (unipolare) abbiamo utilizzato un CD4017 che con un solo pin dell'Arduino ci consente di alimentare in sequenza le quattro fasi del motore.
Come driver di potenza sempre del passo-passo usiamo l'ULN2003 che con esso possiamo alimentare il motore a 12V.
Tra i componenti di ripiego figura lo Shift Register (IC 74HC595) che con solo tre pin del microprocessore visualizziamo con dei led lo stato del sistema.

Per ottenere un effetto "stanga" usiamo due servi (SG90) con i quali possiamo realizzare e controllare uno scivolo sul quale rotolano le palline e sul quale viene realizzata la misura.

Il sistema prevede pure la calibrazione automatica del sistema, se l'apposito switch è in posizione di "Calibrazione" allora vengono realizzate due misure, del bianco e del nero, che fungeranno da estremi per le letture e la classificazione.

Il sensore di colore è di basso costo e viene realizzato tramite una fotoresistenza e tre led che si accendono in sequenza e in base al colore assorbito o riflesso dall'oggetto (rilevato dalla fotoresistenza) il sistema è in grado di definire il colore grazie a degli estremi impostati dall'utente.

La memoria EEPROM viene utilizzata per salvare i valori letti dalla calibrazione per evitare una inutile perdita di dati ad ogni RESET o allo spegnimento del sistema.

Grazie ancora per la lettura e per l'interesse sviluppato che vi ha portato fin qua,
per eventuali chiarimenti, dubbi, malfunzionamenti o consigli prego rivolgersi al sottoscritto scrivendo al seguente indirizzo:  pasettodavide@gmail.com

Enjoy :)
