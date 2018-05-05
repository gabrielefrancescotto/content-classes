
.. _h516a7a2b521825383a3b2b721a727622:

Classi di contenuto per i portali istituzionali
###############################################

.. _h78a33336b592d213d5a132759492a5f:

Verso OntoPiA
#############

.. _h2f65316220271965446c384555203553:

Introduzione
************

.. _h4260697c445014a77736b6b1415d1b:

Un modello dati basato su classi di contenuto
=============================================

I sistemi informativi che \ |LINK1|\  mette a disposizione degli Enti Pubblici (quali ComunWeb, UpipaWeb, SINET template, ecc...) sono basati sulla piattaforma OpenPA, un framework Open Source costituito da un CMS di base (eZ Publish) e da alcune estensioni realizzate ad hoc, che includono strumenti di editing dei contenuti, sistemi per l’importazione e l’esportazione dinamica di dati secondo formati standard e delle componenti per la sincronizzazione delle strutture dati. Tutti i micro-servizi realizzati da Opencontent sono basati su questo tipo di infrastruttura.

\ |IMG1|\ 

Il modello dati della piattaforma si basa sul concetto di \ |STYLE0|\  (\ |STYLE1|\ ), che di fatto gestiscono in forma strutturata le informazioni dei siti web e dei micro-servizi (come OpenAgenda); questo approccio offre numerosi vantaggi alle PA, quali:

* una maggior compatibilità con la \ |STYLE2|\ , per la quale è essenziale che il contenuto sia completamente separato dalla forma

* una \ |STYLE3|\  (form web) per l’inserimento dei contenuti, che aiuta i redattore a validare i contenuti ed a gestirli alla fonte secondo un formato \ |STYLE4|\ 

* rendere qualsiasi tipo di dato disponibile via \ |STYLE5|\ , con benefici conseguenti in termini di interoperabilità e generazione di dataset di alta qualità, aggiornati in tempo reale.

Ogni volta che un ente pubblico decide di dotarsi di questa piattaforma, viene generata una nuova istanza dedicata, con un database indipendente; al 31/12/2017, il numero di istanze di OpenPA erano oltre 300 e le richieste di adesione continuano a crescere.

\ |IMG2|\ 

.. _h6c295c4f51c7b13942f593e4f2a46:

Come si evolvono le classi di contenuto
=======================================

Non essendo stato individuato un modello dati di riferimento in grado di mappare qualsiasi tipo di dato strutturato, le classi di contenuto sono state via via create in base alle necessità degli enti che hanno adottato la piattaforma.

Per garantire che le strutture dati rimangano tra loro allineate nel corso del tempo, è stato predisposto un tool (C&CAF, classes & content alignment framework) che consente di far evolvere le classi di contenuto e al tempo stesso mantenere l’allineamento con le istanze precedentemente attivate.

\ |IMG3|\ 

Pur essendo un modello dati consolidato ed utilizzato da un numero elevato di enti con analoghe esigenze, basato su oltre 250 classi di contenuto, un Ente particolarmente strutturato può manifestare la necessità di gestire nuove tipologie di dati strutturati, richiedendo pertanto una modifica al modello dati, che comporta in particolare la creazione di nuove classi di contenuto o una maggior specializzazione di classi esistenti. 

In accordo con l’Ente, viene aperta una \ |STYLE6|\ , che comporta l’isolamento dell’istanza dal sistema di allineamento automatico. Vengono quindi predisposte le nuove classi di contenuto e sottoposte ai redattori dell’Ente, quindi via via affinate fino a che danno prova di rispondere alle esigenze e alle aspettative. Una volta collaudata, la modifica viene portata in produzione nel repository centrale che tiene in ordine il modello definitivo, quindi applicata automaticamente a tutte le istanze esistenti.

\ |IMG4|\ 

.. _h7f3d1c4f9676b1d376be7d297f133:

Evoluzione del modello secondo le ontologie di AgID (OntoPiA)
=============================================================

Sfruttando il metodo sopra descritto, è in corso un progressivo allineamento con le ontologie ed i vocabolari controllati definiti da AgID:

\ |LINK2|\ 

Si tratta di un repository di ontologie e vocabolari controllati sviluppati da AgID nell'ambito delle azioni previste dal Piano Triennale per l’Informatica.

I microservizi di \ |LINK3|\  utilizzano le API di questo middleware per:

* mappare i contenuti strutturati gestiti dagli enti pubblici secondo le ontologie definite da AgID

* vincolare l'inserimento dei dati ai vocabolari controllati. Ad esempio, l'interfaccia di inserimento dell'indirizzo di un istituto o luogo della cultura, presente in OpenAgenda, utilizza \ |LINK4|\ .

\ |IMG5|\ 

Un esempio concreto di micro-servizio che sfrutta questo paradigma è OpenAgenda.

\ |IMG6|\ 

.. bottom of content


.. |STYLE0| replace:: **classi di contenuto**

.. |STYLE1| replace:: *content classes*

.. |STYLE2| replace:: **multi-canalità**

.. |STYLE3| replace:: **guida**

.. |STYLE4| replace:: *machine-readable*

.. |STYLE5| replace:: **API**

.. |STYLE6| replace:: **iniziativa pilota**


.. |LINK1| raw:: html

    <a href="https://www.opencontent.it/" target="_blank">Opencontent</a>

.. |LINK2| raw:: html

    <a href="https://github.com/italia/daf-ontologie-vocabolari-controllati" target="_blank">https://github.com/italia/daf-ontologie-vocabolari-controllati</a>

.. |LINK3| raw:: html

    <a href="https://www.opencontent.it/Per-la-PA" target="_blank">OpenPA</a>

.. |LINK4| raw:: html

    <a href="http://ontopa.opencontent.it/api/opendata/v2/content/search/classes%20%5Bclassificazione_del_territorio%5D" target="_blank">questa libreria</a>


.. |IMG1| image:: static/Introduzione_1.png
   :height: 430 px
   :width: 642 px

.. |IMG2| image:: static/Introduzione_2.png
   :height: 465 px
   :width: 642 px

.. |IMG3| image:: static/Introduzione_3.png
   :height: 461 px
   :width: 642 px

.. |IMG4| image:: static/Introduzione_4.png
   :height: 500 px
   :width: 642 px

.. |IMG5| image:: static/Introduzione_5.png
   :height: 481 px
   :width: 642 px

.. |IMG6| image:: static/Introduzione_6.png
   :height: 477 px
   :width: 642 px
