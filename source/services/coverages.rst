Coverage
========================
Per "coverage" si intende la rassegna stampa contente gli articoli caricati all'interno della piattaforma iPressLIVE.
Le "coverage" sono organizzate in elementi "catalog" che identificano un set di "coverage", a loro volta le "coverage" contengo i singoli articoli, definiti "coverage item".


Catalog
*******
Gli elementi "catalog" vengono richiamati attraverso una chiave identificativa ("key") 

..  http:example:: curl wget httpie python-requests

    GET /v2/coverages/catalog/<key> HTTP/1.1
    Host: api.ipresslive.com
    Accept: application/json

Parametri query string
Utilizziamo i parametri query string per filtrare e paginare i risultati della chiamata API. 
Il formato per i parametri query string è l'URL completo della risorsa seguito da un punto interrogativo per i parametri facoltativi:

=========   ===============   =========   =======   ================================
Param       Type (length)     Required    Default   Description
=========   ===============   =========   =======   ================================
key 		string(36)        True		            Codice identificativa del "catalog"
=========   ===============   =========   =======   ================================


Risposta

.. code-block:: json

 	{
	   "id":2,
	   "title":"Italia StartUp",
	   "keyPublic":"567da02f-6b5a-4076-8b71-341062b7db78",
	   "keyPrivate":""
	}


