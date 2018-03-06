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

Coverages
**********
Per mostrare le "coverage" contenute all'interno di un catalog si utilizza nuovamente la chiave identificativa dell'elemento catalog ("key")

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


Risposta: il valore del campo scenario dell'elemento "coverage" indicata se si tratta di una rassegna legata ad uno scenario (true) oppure legato ad un brand (false).

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

Coverage
**********
Per mostrare la singola "coverage" occorre utilizzare sia la chiave identificativa dell'elemento catalog ("key") che dell'elemento "coverage".

 ..  http:example:: curl wget httpie python-requests

    GET /v2/catalogs/<key_cat>/coverage/<key_cov> HTTP/1.1
    Host: api.ipresslive.com
    Accept: application/json

Parametri query string
Utilizziamo i parametri query string per filtrare e paginare i risultati della chiamata API. 
Il formato per i parametri query string è l'URL completo della risorsa seguito da un punto interrogativo per i parametri facoltativi:

=========   ===============   =========   =======   ================================
Param       Type (length)     Required    Default   Description
=========   ===============   =========   =======   ================================
key_cat		string(36)        True		            Codice identificativa del "catalog"
key_cov		string(36)        True		            Codice identificativa della "coverage"
page        int               False       1         Mostra la pagina {page} del set di risultati
size        int               False       20        Numero di elementi per pagina
=========   ===============   =========   =======   ================================


Risposta.

.. code-block:: json

 	{
	   "name":"Startup WEB",
	   "page":1,
	   "pages":1375,
	   "elements":[
	      {
	         "id":1389973,
	         "media":"startupitalia.eu",
	         "publishingDate":"2018-03-04T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Tommaso Magrini",
	         "title":"Wi-Fi in aereo, tra offerte e 5G: a che punto siamo",
	         "url":"http://startupitalia.eu/86588-20180304-wi-fi-aereo-offerte-5g-punto"
	      },
	      {
	         "id":1389970,
	         "media":"bresciaoggi.it",
	         "publishingDate":"2018-03-04T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":null,
	         "title":"Start up, la Lombardia regina per le «proposte» innovative",
	         "url":"http://www.bresciaoggi.it/home/economia/start-up-la-lombardia-regina-per-le-proposte-innovative-1.6340481"
	      },
	      {
	         "id":1389976,
	         "media":"thefoodmakers.startupitalia.eu",
	         "publishingDate":"2018-03-03T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Simone Cosimi",
	         "title":"Food delivery: chi c’è, quanto vale, quanti ci lavorano",
	         "url":"http://thefoodmakers.startupitalia.eu/61636-20180303-food-delivery-ce-quanto-vale-quanti-ci-lavorano"
	      },
	      {
	         "id":1389967,
	         "media":"agi.it",
	         "publishingDate":"2018-03-03T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Gianluigi Cogo",
	         "title":"Energia, 5 startup che cambieranno il mondo con la blockchain",
	         "url":"https://www.agi.it/blog-italia/digitale/energia_5_startup_che_cambieranno_il_mondo_con_la_blockchain-3579624/post/2018-03-03/"
	      },
	      {
	         "id":1389975,
	         "media":"primaonline.it",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":null,
	         "title":"Digital Magics apre a Torino e punta Copenaghen, Uk e San Francisco",
	         "url":"http://www.primaonline.it/2018/03/02/267768/digital-magics-apre-a-torino-e-punta-copenaghen-regno-unito-e-san-francisco/"
	      },
	      {
	         "id":1389974,
	         "media":"ilsole24ore.com",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Aliya Ram",
	         "title":"La Francia in lotta con il Regno Unito per la corona europea dell’hi tech ",
	         "url":"http://www.ilsole24ore.com/art/management/2018-01-09/la-francia-lotta-il-regno-unito-la-corona-europea-dell-hi-tech-122242.shtml?uuid=AEfLmQeD"
	      },
	      {
	         "id":1389971,
	         "media":"adnkronos.com",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Vittoria Vimercati",
	         "title":"Fintech, in Italia ha raccolto solo 30 milioni nel 2017",
	         "url":"http://www.adnkronos.com/soldi/finanza/2018/03/02/fintech-italia-raccolto-solo-milioni-nel_7hLA9lnq78wSeNWfGF09DJ.html"
	      },
	      {
	         "id":1389968,
	         "media":"startupitalia.eu",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Anna Gaudenzi",
	         "title":"Let’s change the world. La startup GiPSTech vola in Giappone con NTT DATA",
	         "url":"http://openinnovation.startupitalia.eu/60730-20180302-lets-change-the-world-la-startup-gipstech-vola-giappone-ntt-data"
	      },
	      {
	         "id":1389966,
	         "media":"economyup.it",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Eliana Bentivegna",
	         "title":"eCommerce B2b, ecco 9 startup che aiutano a collegare l’azienda con la sua filiera",
	         "url":"https://www.economyup.it/retail/e-commerce/ecommerce-b2b-9-startup-offrono-soluzioni-connettere-lazienda-la-sua-filiera/"
	      },
	      {
	         "id":1389965,
	         "media":"startupitalia.eu",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Lara Martino",
	         "title":"Manet chiude un round da 1 milione di euro con LVenture Group e Angel Partner Group",
	         "url":"http://startupitalia.eu/86607-20180302-manet-round-lventure-angel-partner-group"
	      },
	      {
	         "id":1389964,
	         "media":"ttgitalia.com",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":null,
	         "title":"Booking.com svela le startup selezionate per Booster ",
	         "url":"https://www.ttgitalia.com/stories/job_talent/140580_bookingcom_svela_le_startup_selezionate_per_booster/"
	      },
	      {
	         "id":1389959,
	         "media":"agi.it",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":null,
	         "title":"Nel 2017 si è investito meno in startup, 208 milioni (ma con quelle all'estero)",
	         "url":"https://www.agi.it/economia/investimenti_startup_2017_aifi-3571159/news/2018-03-02/"
	      },
	      {
	         "id":1389958,
	         "media":"wired.it",
	         "publishingDate":"2018-03-02T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Caterina Maconi",
	         "title":"Venture capital e startup, 5 numeri per capire dove investe l’Italia",
	         "url":"https://www.wired.it/economia/finanza/2018/03/02/venture-capital-startup-italia/"
	      },
	      {
	         "id":1389972,
	         "media":"economyup.it",
	         "publishingDate":"2018-03-01T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Pierluigi Paracchi",
	         "title":"Elezioni 2018, servirebbe un ministro dell’Innovazione ma con portafoglio",
	         "url":"https://www.economyup.it/innovazione/elezioni-2018-servirebbe-un-ministro-dellinnovazione-portafoglio/"
	      },
	      {
	         "id":1389969,
	         "media":"thefoodmakers.startupitalia.eu",
	         "publishingDate":"2018-03-01T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Sara Moraca",
	         "title":"Allergenio, la startup che identifica gli allergeni tra più di 18.000 ingredienti",
	         "url":"http://thefoodmakers.startupitalia.eu/61567-20180301-allergenio-startup-allergeni-ingradienti"
	      },
	      {
	         "id":1389962,
	         "media":"futura.news",
	         "publishingDate":"2018-03-01T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":null,
	         "title":"Yezers, la prima startup politica che vuole migliorare l’Italia",
	         "url":"https://www.futura.news/2018/03/01/yezers-la-prima-startup-politica-che-vuole-migliorare-litalia/"
	      },
	      {
	         "id":1389960,
	         "media":"wired.it",
	         "publishingDate":"2018-03-01T00:00:00",
	         "coverageDate":"2018-03-05T00:00:00",
	         "author":"Diego Barbera",
	         "title":"Le 10 migliori startup del Mobile World Congress",
	         "url":"https://www.wired.it/economia/start-up/2018/03/01/10-migliori-startup-mwc18/"
	      },
	      {
	         "id":1384714,
	         "media":"wired.it",
	         "publishingDate":"2018-02-27T00:00:00",
	         "coverageDate":"2018-02-27T00:00:00",
	         "author":"Antonio Carnevale",
	         "title":" .IT Sezioni Wired Next Fest Gallery Video HOT TOPIC WIRED HEALTH FACEBOOK DIZIONARIO DIGITALE ELEZIONI 2018 GOOGLE MOBILE WORLD CONGRESS 2018… VEDI TUTTI HOME ECONOMIA BUSINESS 350 milioni di export per le pmi italiane che vendono su Amazon",
	         "url":" https://www.wired.it/economia/business/2018/02/26/amazon-export-italia/"
	      },
	      {
	         "id":1384711,
	         "media":"lastampa.it",
	         "publishingDate":"2018-02-27T00:00:00",
	         "coverageDate":"2018-02-27T00:00:00",
	         "author":null,
	         "title":"Sorpresa, startupper non fa rima con giovane",
	         "url":"http://www.lastampa.it/2018/02/27/economia/sorpresa-startupper-non-fa-rima-con-giovane-VGmziIQiEBhccPj2HAtI4L/pagina.html"
	      },
	      {
	         "id":1384690,
	         "media":"wired.it",
	         "publishingDate":"2018-02-27T00:00:00",
	         "coverageDate":"2018-02-27T00:00:00",
	         "author":null,
	         "title":"10 startup italiane che sognano l’America",
	         "url":"https://www.wired.it/economia/start-up/2018/02/23/startup-italia-america/"
	      }
	   ]
	}

