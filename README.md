# Docker
Installa utilizzando lo script di convenienza
Docker fornisce script utili su get.docker.com e test.docker.com per installare versioni edge e di test di Docker Engine - Community in ambienti di sviluppo in modo rapido e non interattivo. Il codice sorgente per gli script si trova nel repository di installazione docker. L'utilizzo di questi script non è consigliato per gli ambienti di produzione e dovresti comprendere i potenziali rischi prima di utilizzarli:
![immagine](https://user-images.githubusercontent.com/56889513/117015574-28b5d380-acf2-11eb-9083-13f149da0e8b.png)

Gli script richiedono i privilegi di root o sudo per essere eseguiti. Pertanto, è necessario esaminare attentamente e controllare gli script prima di eseguirli.
Gli script tentano di rilevare la distribuzione e la versione di Linux e di configurare il sistema di gestione dei pacchetti per te. Inoltre, gli script non consentono di personalizzare alcun parametro di installazione. Ciò potrebbe portare a una configurazione non supportata, dal punto di vista di Docker o dalle linee guida e dagli standard della tua organizzazione.
Gli script installano tutte le dipendenze e le raccomandazioni del gestore di pacchetti senza chiedere conferma. Ciò può installare un gran numero di pacchetti, a seconda della configurazione corrente della macchina host.
Lo script non fornisce opzioni per specificare quale versione di Docker installare e installa l'ultima versione rilasciata nel canale "edge".
Non utilizzare lo script di convenienza se Docker è già stato installato sulla macchina host utilizzando un altro meccanismo.
Questo esempio utilizza lo script su get.docker.com per installare l'ultima versione di Docker Engine - Community su Linux. Per installare l'ultima versione di test, utilizzare invece test.docker.com. In ciascuno dei comandi seguenti, sostituisci ogni occorrenza di get con test.

Avvertimento:

Esaminare sempre gli script scaricati da Internet prima di eseguirli in locale.

$ curl -fsSL https://get.docker.com -o get-docker.sh
$ sudo sh get-docker.sh

<output truncated>
