Coverage
========================
Per "coverage" si intende la rassegna stampa contente gli articoli caricati all'interno della piattaforma iPressLIVE.
Le "coverage" sono organizzate in elementi "catalog" che identificano un set di "coverage", a loro volta le "coverage" contengo i singoli articoli, definiti "coverage item".


Catalog
*******
Gli elementi "catalog" vengono richiamati attraverso una chiave identificativa ("key") 

..  http:example:: curl wget httpie python-requests

    GET /v2/catalogs/<key> HTTP/1.1
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

Coverage
********
Per mostrare le "coverage" contenute all'interno di un catalog si utilizza nuovamente la chiave identificativa catalogo "key"

 ..  http:example:: curl wget httpie python-requests

    GET /v2/catalogs/<key>/coverages HTTP/1.1
    Host: api.ipresslive.com
    Accept: application/json

Parametri query string
Utilizziamo i parametri query string per filtrare e paginare i risultati della chiamata API. 
Il formato per i parametri query string è l'URL completo della risorsa seguito da un punto interrogativo per i parametri facoltativi:

=========   ===============   =========   =======   ================================
Param       Type (length)     Required    Default   Description
=========   ===============   =========   =======   ================================
key 		string(36)        True		            Codice identificativa del "catalog"
page        int               False       1         Mostra la pagina {page} del set di risultati
size        int               False       20        Numero di elementi per pagina
=========   ===============   =========   =======   ================================


Risposta
Il valore del campo scenario dell'elemento "coverage" indicata se si tratta di una rassegna legata ad uno scenario (true) oppure legato ad un brand (false).

.. code-block:: json

 	{
	   "name":"Italia StartUp",
	   "page":1,
	   "pages":1,
	   "elements":[
	      {
	         "id":12,
	         "title":"Startup",
	         "keyPublic":"7157fc3f-55f3-4dae-8dd4-b7f470f79bc0",
	         "keyPrivate":"",
	         "scenario":true
	      },
	      {
	         "id":138,
	         "title":"Startup WEB",
	         "keyPublic":"443a96ae-93b7-402f-8437-12493c3ce026",
	         "keyPrivate":"",
	         "scenario":true
	      },
	      {
	         "id":13,
	         "title":"Italia Startup",
	         "keyPublic":"b8a96a5f-62d6-4b09-8edb-4dd4404ba02b",
	         "keyPrivate":"",
	         "scenario":false
	      },
	      {
	         "id":27,
	         "title":"Italia Startup - web",
	         "keyPublic":"ef68dfa3-ac0c-4287-a03f-8e1b424e8b80",
	         "keyPrivate":"",
	         "scenario":false
	      },
	      {
	         "id":68,
	         "title":"Italia Startup Radio",
	         "keyPublic":"92be179b-0ba4-4b32-a486-626b24e3bdc0",
	         "keyPrivate":"",
	         "scenario":false
	      },
	      {
	         "id":69,
	         "title":"Italia Startup TV",
	         "keyPublic":"80b70620-ddc1-4e95-bc13-a4d8a649597e",
	         "keyPrivate":"",
	         "scenario":false
	      }
	   ]
	}


