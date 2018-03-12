Event
========================
Per "event" si intendono gli eventi caricati all'interno della piattaforma iPressLIVE.
Gli eventi sono rappresentati all'interno della piattaforma come delle Simple Application Page costituite da un insieme di "Section". Ogni "Section" o sezione ha un proprio insieme di entità figlio a seconda degli elementi renderizzati


Events
*******
Gli elementi "catalog" vengono richiamati attraverso una chiave identificativa ("key") 

..  http:example:: curl wget httpie python-requests

    GET /v2/events/ HTTP/1.1
    Host: api.ipresslive.com
    Accept: application/json

arametri query string
Utilizziamo i parametri query string per filtrare e paginare i risultati della chiamata API. 
Il formato per i parametri query string è l'URL completo della risorsa seguito da un punto interrogativo per i parametri facoltativi:

=========   ===============   =========   =======   ================================
Param       Type (length)     Required    Default   Description
=========   ===============   =========   =======   ================================
lang        string(2)         False       it        Filtra gli elementi per lingua (formato ISO short)
page        int               False       1         Mostra la pagina {page} del set di risultati
size        int               False       20        Numero di elementi per pagina
search      string            False                 Filtra gli elementi facendo una ricerca per keyword
=========   ===============   =========   =======   ================================


Risposta

.. code-block:: json

 	{
	   "name":null,
	   "page":1,
	   "pages":4,
	   "elements":[
	      {
	         "id":118,
	         "name":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Mobile Payment & Commerce ",
	         "banner":{
	            "id":55253,
	            "size":143779,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20182/737f91cd-6a56-41f3-934e-854f77c1f92b__O.png",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Mobile Payment & Commerce "
	         },
	         "header":{
	            "id":55089,
	            "size":62788,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20181/0894b60e-e6c9-4340-b79b-a6c3c28c18b6__O.png",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Mobile Payment & Commerce "
	         },
	         "sections":null,
	         "startDate":"2018-03-07T00:00:00",
	         "endDate":"2018-03-07T00:00:00",
	         "time":"9-13",
	         "latitude":"45.5031585",
	         "longitude":"9.15741980000007"
	      },
	      {
	         "id":120,
	         "name":"Nasce a Milano il primo centro internazionale per la cultura digitale",
	         "banner":{
	            "id":55259,
	            "size":131436,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20182/79adc5dd-09c2-4892-b345-2729399b76e2__O.jpg",
	            "caption":"Nasce a Milano il primo centro internazionale per la cultura digitale"
	         },
	         "header":{
	            "id":55258,
	            "size":244551,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20182/cddc9468-2a94-49f0-a311-5a688beec7da__O.jpg",
	            "caption":"Nasce a Milano il primo centro internazionale per la cultura digitale"
	         },
	         "sections":null,
	         "startDate":"2018-02-26T00:00:00",
	         "endDate":null,
	         "time":"10:00",
	         "latitude":"45.472752",
	         "longitude":"9.182821999999987"
	      },
	      {
	         "id":117,
	         "name":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Mobile B2c Strategy",
	         "banner":{
	            "id":55085,
	            "size":57168,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20181/50f59c51-52d1-49e9-a46c-b3afd6e2c78c__O.png",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Mobile B2c Strategy"
	         },
	         "header":{
	            "id":55080,
	            "size":63956,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20181/4c6e528e-5fe3-4ff7-92a0-71d0d49375d6__O.png",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Mobile B2c Strategy"
	         },
	         "sections":null,
	         "startDate":"2018-02-14T00:00:00",
	         "endDate":"2018-02-14T00:00:00",
	         "time":"9.30 - 13.00 ",
	         "latitude":"45.503245",
	         "longitude":"9.157193000000007"
	      },
	      {
	         "id":114,
	         "name":"Open Summit 2017",
	         "banner":{
	            "id":54805,
	            "size":46167,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201712/55e5b974-0d32-4d9f-955f-c44ed6783616__O.jpg",
	            "caption":"Open Summit 2017"
	         },
	         "header":{
	            "id":54804,
	            "size":126731,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201712/a6e72f10-e002-4967-b494-8aede20ac938__O.jpg",
	            "caption":"Open Summit 2017"
	         },
	         "sections":null,
	         "startDate":"2017-12-18T00:00:00",
	         "endDate":null,
	         "time":"8:45 - 22:45",
	         "latitude":"45.4605557",
	         "longitude":"9.227540299999987"
	      },
	      {
	         "id":109,
	         "name":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Omnichannel Customer Experience",
	         "banner":{
	            "id":54049,
	            "size":78791,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/67d558fa-ca60-4ddd-b5c4-96a79bab28e9__O.png",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Omnichannel Customer Experience"
	         },
	         "header":{
	            "id":54037,
	            "size":56471,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/6a694da5-740d-4499-a1db-5f6a6996be47__O.jpg",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Omnichannel Customer Experience"
	         },
	         "sections":null,
	         "startDate":"2017-11-21T00:00:00",
	         "endDate":"2017-11-21T00:00:00",
	         "time":"9.30 - 13.30",
	         "latitude":"45.5035422",
	         "longitude":"9.15644599999996"
	      },
	      {
	         "id":107,
	         "name":"TRAP 2017",
	         "banner":{
	            "id":53903,
	            "size":137193,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/b3fb6945-4f1d-4cee-b0b7-88f73e84d54d__O.jpg",
	            "caption":"TRAP 2017"
	         },
	         "header":{
	            "id":53902,
	            "size":137193,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/c12554eb-02e6-4aea-935a-a4943582e444__O.jpg",
	            "caption":"TRAP 2017"
	         },
	         "sections":null,
	         "startDate":"2017-10-25T00:00:00",
	         "endDate":"2017-10-26T00:00:00",
	         "time":null,
	         "latitude":"41.8501915",
	         "longitude":"12.572766000000001"
	      },
	      {
	         "id":103,
	         "name":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Innovazione Digitale nel Turismo",
	         "banner":{
	            "id":53490,
	            "size":142009,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/3bcfb102-9aa3-4150-84b1-6f76088821e9__O.png",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Innovazione Digitale nel Turismo"
	         },
	         "header":{
	            "id":53489,
	            "size":142009,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/6d5e251e-0243-4916-a9d9-20fb86c23325__O.png",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Innovazione Digitale nel Turismo"
	         },
	         "sections":null,
	         "startDate":"2017-10-13T00:00:00",
	         "endDate":"2017-10-13T00:00:00",
	         "time":"10.30 - 13.30",
	         "latitude":"44.0723588",
	         "longitude":"12.526416499999982"
	      },
	      {
	         "id":101,
	         "name":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio eCommerce B2c ",
	         "banner":{
	            "id":52378,
	            "size":93264,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20179/bf61305e-b057-469f-a079-e11897d822b1__O.jpg",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio eCommerce B2c "
	         },
	         "header":{
	            "id":52283,
	            "size":56571,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20179/f8fab9c7-c7ea-415b-a01f-f74bb4079d42__O.jpg",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio eCommerce B2c "
	         },
	         "sections":null,
	         "startDate":"2017-10-10T00:00:00",
	         "endDate":"2017-10-11T00:00:00",
	         "time":"09.00 - 13.00",
	         "latitude":"45.51844639999999",
	         "longitude":"9.213105700000028"
	      },
	      {
	         "id":88,
	         "name":"Hack Developers Italia",
	         "banner":{
	            "id":52011,
	            "size":49913,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20179/710e5776-094b-4bce-9a88-9f52164eab1a__O.jpg",
	            "caption":"Hack Developers Italia"
	         },
	         "header":{
	            "id":52010,
	            "size":117416,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20179/e1a05038-830b-4206-99bb-77025814109c__O.jpg",
	            "caption":"Hack Developers Italia"
	         },
	         "sections":null,
	         "startDate":"2017-10-07T00:00:00",
	         "endDate":"2017-10-08T00:00:00",
	         "time":null,
	         "latitude":"45.4840705",
	         "longitude":"9.175455100000022"
	      },
	      {
	         "id":92,
	         "name":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Cloud & ICT as a Service ",
	         "banner":{
	            "id":52379,
	            "size":147596,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20179/582f1b9d-12d3-4e7d-a582-873a887423fc__O.jpg",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Cloud & ICT as a Service "
	         },
	         "header":{
	            "id":52282,
	            "size":54264,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20179/90e4f72e-0569-421a-972d-915f0e3c6ccb__O.jpg",
	            "caption":"Convegno di presentazione dei risultati della Ricerca dell'Osservatorio Cloud & ICT as a Service "
	         },
	         "sections":null,
	         "startDate":"2017-10-04T00:00:00",
	         "endDate":"2017-10-04T00:00:00",
	         "time":"09.30 - 13.00",
	         "latitude":"45.503091",
	         "longitude":"9.156407100000024"
	      },
	      {
	         "id":100,
	         "name":"Un Natale da favola",
	         "banner":{
	            "id":53068,
	            "size":37375,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/8b69e853-0e7d-49b3-ac03-7828ead5edb3__O.jpg",
	            "caption":"Un Natale da favola"
	         },
	         "header":{
	            "id":54231,
	            "size":197,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201711/93116575-429b-42d3-afa4-624bc698840d__O.png",
	            "caption":"Un Natale da favola"
	         },
	         "sections":null,
	         "startDate":"2017-10-04T00:00:00",
	         "endDate":"2017-10-04T00:00:00",
	         "time":" 12.00 - 21.00",
	         "latitude":"45.4668855",
	         "longitude":"9.166375300000027"
	      },
	      {
	         "id":106,
	         "name":"B4DPA Bocconi for Digital Public Administration Award",
	         "banner":{
	            "id":52889,
	            "size":48719,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/431faa7c-f82d-4ed4-b01b-c68069e877ae__O.jpg",
	            "caption":"B4DPA Bocconi for Digital Public Administration Award"
	         },
	         "header":{
	            "id":52888,
	            "size":48719,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/201710/6d511074-7e4c-435a-a094-ff5922b7fcf6__O.jpg",
	            "caption":"B4DPA Bocconi for Digital Public Administration Award"
	         },
	         "sections":null,
	         "startDate":"2017-10-02T00:00:00",
	         "endDate":null,
	         "time":null,
	         "latitude":"45.4654219",
	         "longitude":"9.18592430000001"
	      },
	      {
	         "id":90,
	         "name":"I-7 Innovators’ Strategic Advisory Board on People-Centered Innovation",
	         "banner":{
	            "id":51973,
	            "size":68571,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20179/94125380-cbf8-4660-abbc-f16ffa17fbb5__O.jpg",
	            "caption":"I-7 Innovators’ Strategic Advisory Board on People-Centered Innovation"
	         },
	         "header":{
	            "id":51972,
	            "size":194228,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20179/d630b5f6-9ab4-4702-82f2-f328f1bc5bbb__O.jpg",
	            "caption":"I-7 Innovators’ Strategic Advisory Board on People-Centered Innovation"
	         },
	         "sections":null,
	         "startDate":"2017-09-25T00:00:00",
	         "endDate":null,
	         "time":null,
	         "latitude":"45.4654219",
	         "longitude":"9.18592430000001"
	      },
	      {
	         "id":87,
	         "name":"IL PIANO NAZIONALE SCUOLA DIGITALE INCONTRA IL PAESE",
	         "banner":{
	            "id":51738,
	            "size":52341,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20177/27b9ca4c-ce18-4905-a823-81a714101452__O.jpg",
	            "caption":"IL PIANO NAZIONALE SCUOLA DIGITALE INCONTRA IL PAESE"
	         },
	         "header":{
	            "id":51737,
	            "size":113612,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20177/4ace7a31-73a0-4aec-b393-bd7b11b507dd__O.jpg",
	            "caption":"IL PIANO NAZIONALE SCUOLA DIGITALE INCONTRA IL PAESE"
	         },
	         "sections":null,
	         "startDate":"2017-07-26T00:00:00",
	         "endDate":null,
	         "time":null,
	         "latitude":"41.8976887",
	         "longitude":"12.502488200000016"
	      },
	      {
	         "id":74,
	         "name":"Campus Party 2017",
	         "banner":{
	            "id":41328,
	            "size":153403,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20176/48108fa4-d435-48e4-8ab7-b743f994b1c1__O.jpg",
	            "caption":"Campus Party 2017"
	         },
	         "header":{
	            "id":41327,
	            "size":94648,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20176/cc92d0ca-9d37-484a-8ef4-78481e94f3b3__O.jpg",
	            "caption":"Campus Party 2017"
	         },
	         "sections":null,
	         "startDate":"2017-07-20T00:00:00",
	         "endDate":"2017-07-23T00:00:00",
	         "time":"a partire dalle ore 12:00",
	         "latitude":"45.48092",
	         "longitude":"9.1533498"
	      },
	      {
	         "id":85,
	         "name":"Il Piano Triennale: verso il sistema operativo del Paese - Luiss Enlabs - mercoledì 5 luglio 2017",
	         "banner":{
	            "id":51557,
	            "size":639772,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20177/c62cb59c-971f-407e-a672-3b85d75007e5__O.png",
	            "caption":"Il Piano Triennale: verso il sistema operativo del Paese - Luiss Enlabs - mercoledì 5 luglio 2017"
	         },
	         "header":{
	            "id":51633,
	            "size":639772,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20177/8b382345-a284-4711-930a-11749ac134d0__O.png",
	            "caption":"Il Piano Triennale: verso il sistema operativo del Paese - Luiss Enlabs - mercoledì 5 luglio 2017"
	         },
	         "sections":null,
	         "startDate":"2017-07-05T00:00:00",
	         "endDate":null,
	         "time":"8:30 - 18:15",
	         "latitude":"41.9015448",
	         "longitude":"12.503105600000026"
	      },
	      {
	         "id":82,
	         "name":"Convegno di presentazione dei risultati della ricerca sul Food&Grocery dell’osservatorio ecommerce B2C",
	         "banner":{
	            "id":41356,
	            "size":55433,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20176/063112cc-9006-48e2-a711-d9fbcdfed4bf__O.jpg",
	            "caption":"Convegno di presentazione dei risultati della ricerca sul Food&Grocery dell’osservatorio ecommerce B2C"
	         },
	         "header":{
	            "id":41355,
	            "size":41429,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20176/f3deb24f-ffdb-490d-bfc1-921e24e5b205__O.jpg",
	            "caption":"Convegno di presentazione dei risultati della ricerca sul Food&Grocery dell’osservatorio ecommerce B2C"
	         },
	         "sections":null,
	         "startDate":"2017-06-28T00:00:00",
	         "endDate":null,
	         "time":null,
	         "latitude":"45.5031126",
	         "longitude":"9.156153700000004"
	      },
	      {
	         "id":79,
	         "name":"Digital Design Days 2017",
	         "banner":{
	            "id":40672,
	            "size":485200,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20175/c30b632b-01e2-4680-984e-d1ff958f5d5e__O.png",
	            "caption":"Digital Design Days 2017"
	         },
	         "header":{
	            "id":40671,
	            "size":863168,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20175/a288eccc-19d5-4047-8123-71c936ab7f3d__O.png",
	            "caption":"Digital Design Days 2017"
	         },
	         "sections":null,
	         "startDate":"2017-06-01T00:00:00",
	         "endDate":null,
	         "time":"13.30 - 14.00",
	         "latitude":"45.4840705",
	         "longitude":"9.175455100000022"
	      },
	      {
	         "id":81,
	         "name":"BIZ Factory ",
	         "banner":{
	            "id":40864,
	            "size":41951,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20175/7af82804-98bc-4d81-9a24-fe37f805e5c7__O.png",
	            "caption":"BIZ Factory "
	         },
	         "header":{
	            "id":40863,
	            "size":41951,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20175/bb6656ef-b149-45c7-a80b-51962ab94ce8__O.png",
	            "caption":"BIZ Factory "
	         },
	         "sections":null,
	         "startDate":"2017-05-31T00:00:00",
	         "endDate":"2017-06-06T00:00:00",
	         "time":"10.00",
	         "latitude":"45.4441171",
	         "longitude":"9.20847839999999"
	      },
	      {
	         "id":78,
	         "name":"Forum Pa 2017",
	         "banner":{
	            "id":40596,
	            "size":36167,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20175/3264a8d8-8dc6-4b01-a399-131ef37ca913__O.jpg",
	            "caption":"Forum Pa 2017"
	         },
	         "header":{
	            "id":40595,
	            "size":81523,
	            "default":false,
	            "xsmall":null,
	            "small":null,
	            "medium":null,
	            "large":null,
	            "link":"https://s3.amazonaws.com/iprs/files/events/header/20175/30926742-903f-4654-be72-c3333b8a168e__O.jpg",
	            "caption":"Forum Pa 2017"
	         },
	         "sections":null,
	         "startDate":"2017-05-23T00:00:00",
	         "endDate":"2017-05-25T00:00:00",
	         "time":null,
	         "latitude":"41.83087769999999",
	         "longitude":"12.472078900000042"
	      }
	   ]
	}


