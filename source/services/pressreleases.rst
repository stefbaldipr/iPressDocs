Press Release
========================
Per "press release" si intendono le news o i comunicati stampa caricati all'interno della piattaforma iPressLIVE.

List
*****
Le liste o elementi "list" permettono di creare un elenco di "press release" facilmente personalizzabile all'interno della piattaforma iPressLIVE.

..  http:example:: curl wget httpie python-requests

    GET /v2/pressreleases/list/<code> HTTP/1.1
    Host: api.ipresslive.com
    Accept: application/json

Parametri query string
Utilizziamo i parametri query string per filtrare e paginare i risultati della chiamata API. 
Il formato per i parametri query string è l'URL completo della risorsa seguito da un punto interrogativo per i parametri facoltativi:

=========   ===============   =========   =======   ================================
Param       Type (length)     Required    Default   Description
=========   ===============   =========   =======   ================================
code		string(36)        True		            Codice identificativo della lista
lang        string(2)         False                 Filtra gli elementi per lingua (formato ISO short)
page        int               False       1         Mostra la pagina {page} del set di risultati
size        int               False       20        Numero di elementi per pagina
=========   ===============   =========   =======   ================================


Risposta

.. code-block:: json

 	{
	   "name":"amazon",
	   "page":1,
	   "pages":20,
	   "elements":[
	      {
	         "id":24894,
	         "title":"Le città che leggono di più secondo Amazon.it",
	         "summary":"Per il quinto anno consecutivo Milano conquista la prima posizione, confermandosi la città che in assoluto acquista maggiormente libri ed eBook su Amazon.it. Triveneto sempre protagonista: quest’anno Trieste ottiene il secondo posto, Padova il terzo e Trento il quinto. Cresce Bologna, quarta, e Torino entra nella top 10.\r\nBolzano preferisce i romanzi rosa, Firenze seconda per i libri di viaggio\r\n",
	         "publishDate":"2017-08-16T09:00:00",
	         "createDate":"2017-08-09T15:04:00",
	         "publishedBy":"Irene Artemagni e Marco Ferrario per Amazon Italia",
	         "link":"http://www.ipresslive.it/comunicates/24894/le-citta-che-leggono-di-piu-secondo-amazonit",
	         "shortlink":"http://iprs.es/c/24894",
	         "content":null,
	         "defaultImage":{
	            "id":51884,
	            "size":651540,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20178/d77c943a-8629-47fe-a6f3-57f32508e1af__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20178/d77c943a-8629-47fe-a6f3-57f32508e1af__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20178/d77c943a-8629-47fe-a6f3-57f32508e1af__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20178/d77c943a-8629-47fe-a6f3-57f32508e1af__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20178/d77c943a-8629-47fe-a6f3-57f32508e1af__O.jpg",
	            "caption":"Milano"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Attualità"
	            },
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Cultura"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Editoria"
	            },
	            {
	               "name":"Femminile"
	            },
	            {
	               "name":"Giovani"
	            },
	            {
	               "name":"Libri"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            },
	            {
	               "name":"Vetrine/Shopping"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":24889,
	         "title":"Cosa leggono i VIP? I libri preferiti dei Baustelle, Nek, Omar Pedrini, Gabriele Mainetti e Guè Pequeno",
	         "summary":" Amazon.it aggiorna le classifiche dei libri preferiti da personaggi famosi in Italia L’iniziativa che ha come scopo ispirare e incentivare i giovani ad avvicinarsi al mondo della lettura procede proponendo 5 nuovi personaggi ",
	         "publishDate":"2017-08-02T12:00:00",
	         "createDate":"2017-08-02T13:57:00",
	         "publishedBy":"Anna Meini e Giulia Perfetti per Amazon Italia ",
	         "link":"http://www.ipresslive.it/comunicates/24889/cosa-leggono-i-vip-i-libri-preferiti-dei-baustelle-nek-omar-pedrini-gabriele-mainetti-e-gue-pequeno",
	         "shortlink":"http://iprs.es/c/24889",
	         "content":null,
	         "defaultImage":{
	            "id":51859,
	            "size":100536,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20178/c1dae3dd-c0e3-4aff-9657-d57ea0018650__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20178/c1dae3dd-c0e3-4aff-9657-d57ea0018650__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20178/c1dae3dd-c0e3-4aff-9657-d57ea0018650__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20178/c1dae3dd-c0e3-4aff-9657-d57ea0018650__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20178/c1dae3dd-c0e3-4aff-9657-d57ea0018650__O.jpg",
	            "caption":"Baustelle. Foto Credits: Baustelle Facebook"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Cinema"
	            },
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Consumatori"
	            },
	            {
	               "name":"Costume"
	            },
	            {
	               "name":"Femminile"
	            },
	            {
	               "name":"Giovani"
	            },
	            {
	               "name":"Hobby e tempo libero"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Locale"
	            },
	            {
	               "name":"Maschile"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":24866,
	         "title":"Migliaia i prodotti e 15% di sconto sui testi scolastici: Amazon.it lancia Amazon 15 e lode e si prepara al back to school",
	         "summary":"Settembre si avvicina, gli studenti e i loro genitori tornano a caccia del diario e dello zaino preferito: Amazon è pronta ad accoglierli con una vasta selezione di prodotti in un negozio ad hoc pensato per loro: www.amazon.it/ritorno-a-scuola\r\n\r\nAl via anche l’operazione Amazon 15 e Lode, che consente di ricevere a casa i testi scolastici con lo sconto del 15% ed effettuare in pochi click l’ordine complessivo di tutti i libri previsti per la classe dei figli",
	         "publishDate":"2017-07-20T10:00:00",
	         "createDate":"2017-07-20T10:11:00",
	         "publishedBy":"Irene Artemagni per Amazon.it",
	         "link":"http://www.ipresslive.it/comunicates/24866/migliaia-i-prodotti-e-15-di-sconto-sui-testi-scolastici-amazonit-lancia-amazon-15-e-lode-e-si-prepara-al-back-to-school",
	         "shortlink":"http://iprs.es/c/24866",
	         "content":null,
	         "defaultImage":{
	            "id":51718,
	            "size":49570,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20177/68262931-3b28-46a9-a426-a455fedce118__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20177/68262931-3b28-46a9-a426-a455fedce118__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20177/68262931-3b28-46a9-a426-a455fedce118__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20177/68262931-3b28-46a9-a426-a455fedce118__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20177/68262931-3b28-46a9-a426-a455fedce118__O.jpg",
	            "caption":"Amazon.it lancia Amazon 15 e lode e si prepara al back to school"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Cultura"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Familiare"
	            },
	            {
	               "name":"Femminile"
	            },
	            {
	               "name":"Giovani"
	            },
	            {
	               "name":"Libri"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":24850,
	         "title":"Prime Day 2017 è stata la più grande giornata di shopping di sempre su Amazon.it",
	         "summary":"Centinaia di venditori terzi hanno partecipato al Prime Day 2017 su Amazon.it \r\nIl prodotto più venduto su Prime Now a Milano, durante il Prime Day 2017, è stato l’Hamburger di Scottona - Chianina IGP",
	         "publishDate":"2017-07-12T13:00:00",
	         "createDate":"2017-07-12T16:08:00",
	         "publishedBy":"Marco Ferrario per Amazon.it",
	         "link":"http://www.ipresslive.it/comunicates/24850/prime-day-2017-e-stata-la-piu-grande-giornata-di-shopping-di-sempre-su-amazonit",
	         "shortlink":"http://iprs.es/c/24850",
	         "content":null,
	         "defaultImage":{
	            "id":51641,
	            "size":157025,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20177/85987624-6d19-42e9-8b6c-7515db3ef2d9__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20177/85987624-6d19-42e9-8b6c-7515db3ef2d9__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20177/85987624-6d19-42e9-8b6c-7515db3ef2d9__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20177/85987624-6d19-42e9-8b6c-7515db3ef2d9__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20177/85987624-6d19-42e9-8b6c-7515db3ef2d9__O.jpg",
	            "caption":"Pastiglie Finish All in One Max 110 Lemon: tra i prodotti in promozione più acquistati in Italia "
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Accessori Moda"
	            },
	            {
	               "name":"Attualità"
	            },
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Consumatori"
	            },
	            {
	               "name":"Corporate e Finanza"
	            },
	            {
	               "name":"Distribuzione"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Economia"
	            },
	            {
	               "name":"Elettronica"
	            },
	            {
	               "name":"Familiare"
	            },
	            {
	               "name":"Femminile"
	            },
	            {
	               "name":"Fotografia"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Logistica"
	            },
	            {
	               "name":"Maschile"
	            },
	            {
	               "name":"Vetrine/Shopping"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":24843,
	         "title":"Il Prime Day 2017 di Amazon offre ai clienti Prime una grandiosa giornata di promozioni dedicate a tutte le loro passioni ",
	         "summary":"I clienti Prime possono iniziare ad acquistare tra migliaia di promozioni a partire dalle 18:00 di oggi, con nuove occasioni di risparmio a loro riservate per 30 ore di fila. In Italia il numero delle offerte di Prime Day da parte dei venditori terzi è cresciuto dell’80% rispetto al 2016.\r\nIn occasione di Prime Day, i clienti Prime di Milano, potranno accedere a centinaia di promozioni con consegna gratuita in due ore con Prime Now, oltre a una selezione esclusiva di Carni dal Mondo e di special",
	         "publishDate":"2017-07-10T09:00:00",
	         "createDate":"2017-07-09T17:15:00",
	         "publishedBy":"Marco Ferrario e Irene Artemagni per Amazon Italia",
	         "link":"http://www.ipresslive.it/comunicates/24843/il-prime-day-2017-di-amazon-offre-ai-clienti-prime-una-grandiosa-giornata-di-promozioni-dedicate-a-tutte-le-loro-passioni",
	         "shortlink":"http://iprs.es/c/24843",
	         "content":null,
	         "defaultImage":{
	            "id":51601,
	            "size":86761,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20177/0759adc8-fe1d-4d07-8555-90793ac46d13__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20177/0759adc8-fe1d-4d07-8555-90793ac46d13__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20177/0759adc8-fe1d-4d07-8555-90793ac46d13__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20177/0759adc8-fe1d-4d07-8555-90793ac46d13__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20177/0759adc8-fe1d-4d07-8555-90793ac46d13__O.jpg",
	            "caption":"Prime Day 2017"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Beauty"
	            },
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Consumatori"
	            },
	            {
	               "name":"Distribuzione"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Economia"
	            },
	            {
	               "name":"Hobby e tempo libero"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            },
	            {
	               "name":"Video"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":24842,
	         "title":"Con Prime Now le promozioni di Prime Day arrivano prima: centinaia di prodotti con consegna gratuita in due ore ",
	         "summary":"In occasione di Prime Day, i clienti Prime di Milano e 46 comuni dell’hinterland, potranno accedere a centinaia di promozioni con consegna gratuita in due ore con Prime Now\r\n\r\nDurante le 30 ore di Prime Day, i clienti Prime che utilizzeranno per la prima volta Prime Now riceveranno uno sconto di €20 sul loro primo ordine, inserendo il codice promozionale PRIMENOW20\r\nTutti pronti per le grigliate estive con il 25% di sconto su una selezione di carni italiane e internazionali, ma anche promozion",
	         "publishDate":"2017-07-07T09:00:00",
	         "createDate":"2017-07-07T09:40:00",
	         "publishedBy":"Marco Ferrario e Irene Artemagni per Amazon",
	         "link":"http://www.ipresslive.it/comunicates/24842/con-prime-now-le-promozioni-di-prime-day-arrivano-prima-centinaia-di-prodotti-con-consegna-gratuita-in-due-ore",
	         "shortlink":"http://iprs.es/c/24842",
	         "content":null,
	         "defaultImage":{
	            "id":51576,
	            "size":62623,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20177/804f3845-b92a-4b34-907d-0e845ca5cf63__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20177/804f3845-b92a-4b34-907d-0e845ca5cf63__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20177/804f3845-b92a-4b34-907d-0e845ca5cf63__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20177/804f3845-b92a-4b34-907d-0e845ca5cf63__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20177/804f3845-b92a-4b34-907d-0e845ca5cf63__O.jpg",
	            "caption":"Prime Day a Milano | Con Amazon Prime Now, centinaia di promozioni tra cui Carni dal mondo e specialità regionali"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"App"
	            },
	            {
	               "name":"Consumatori"
	            },
	            {
	               "name":"Distribuzione"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Food & Beverage"
	            },
	            {
	               "name":"Locale"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":24833,
	         "title":"Su Amazon i venditori terzi si preparano alle vendite record del Prime Day",
	         "summary":"I venditori terzi colgono l'occasione del Prime Day per raggiungere nuovi clienti, lanciare nuovi prodotti e aumentare le vendite.\r\nDurante il Prime Day dello scorso anno, a livello globale, i clienti hanno ordinato oltre 20 milioni di articoli da venditori terzi.\r\nRispetto allo scorso anno in Italia il numero delle offerte di Prime Day da parte dei venditori crescerà dell’80%\r\n",
	         "publishDate":"2017-07-06T10:00:00",
	         "createDate":"2017-07-06T10:43:00",
	         "publishedBy":"Marco Ferrario e Giulia Perfetti per Amazon",
	         "link":"http://www.ipresslive.it/comunicates/24833/su-amazon-i-venditori-terzi-si-preparano-alle-vendite-record-del-prime-day",
	         "shortlink":"http://iprs.es/c/24833",
	         "content":null,
	         "defaultImage":{
	            "id":51545,
	            "size":60823,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20177/3c142d7a-5fde-431a-856b-d7755a60b45c__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20177/3c142d7a-5fde-431a-856b-d7755a60b45c__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20177/3c142d7a-5fde-431a-856b-d7755a60b45c__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20177/3c142d7a-5fde-431a-856b-d7755a60b45c__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20177/3c142d7a-5fde-431a-856b-d7755a60b45c__O.jpg",
	            "caption":"Polaroid Fotocamera Digitale SnapTouch a Stampa Istantanea "
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Costume"
	            },
	            {
	               "name":"Distribuzione"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Economia"
	            },
	            {
	               "name":"Elettronica"
	            },
	            {
	               "name":"Food & Beverage"
	            },
	            {
	               "name":"Fotografia"
	            },
	            {
	               "name":"Moda"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            },
	            {
	               "name":"Vetrine/Shopping"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":24829,
	         "title":"#AmazonPublishing e #AmazonCrossing: 8 nuovi titoli per l’estate e tante offerte in vista del Prime Day ",
	         "summary":"",
	         "publishDate":"2017-07-05T12:00:00",
	         "createDate":"2017-07-05T12:51:00",
	         "publishedBy":"",
	         "link":"http://www.ipresslive.it/comunicates/24829/amazonpublishing-e-amazoncrossing-8-nuovi-titoli-per-lestate-e-tante-offerte-in-vista-del-prime-day",
	         "shortlink":"http://iprs.es/c/24829",
	         "content":null,
	         "defaultImage":{
	            "id":51624,
	            "size":37522,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20177/dd0e5398-0e89-465b-a9fd-4bb29fdae33c__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20177/dd0e5398-0e89-465b-a9fd-4bb29fdae33c__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20177/dd0e5398-0e89-465b-a9fd-4bb29fdae33c__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20177/dd0e5398-0e89-465b-a9fd-4bb29fdae33c__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20177/dd0e5398-0e89-465b-a9fd-4bb29fdae33c__O.jpg",
	            "caption":"Un cuore oscuro."
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Editoria"
	            },
	            {
	               "name":"Libri"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14825,
	         "title":"Cosa leggono i VIP? I 10 libri preferiti di Andrea Dovizioso, Tiziano Ferro, Benedetta Parodi e Paola Turci",
	         "summary":"Amazon.it svela le classifiche dei 10 libri preferiti da personaggi celebri. Si tratta di un’iniziativa che ha come scopo di ispirare e incentivare i giovani ad avvicinarsi al mondo della lettura.",
	         "publishDate":"2017-07-03T11:00:00",
	         "createDate":"2017-07-03T11:22:00",
	         "publishedBy":"Irene Artemagni per Amazon.it",
	         "link":"http://www.ipresslive.it/comunicates/14825/cosa-leggono-i-vip-i-10-libri-preferiti-di-andrea-dovizioso-tiziano-ferro-benedetta-parodi-e-paola-turci",
	         "shortlink":"http://iprs.es/c/14825",
	         "content":null,
	         "defaultImage":{
	            "id":41497,
	            "size":1564603,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20177/bb34b2e2-d1fc-425d-b732-1349182bdd0e__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20177/bb34b2e2-d1fc-425d-b732-1349182bdd0e__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20177/bb34b2e2-d1fc-425d-b732-1349182bdd0e__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20177/bb34b2e2-d1fc-425d-b732-1349182bdd0e__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20177/bb34b2e2-d1fc-425d-b732-1349182bdd0e__O.jpg",
	            "caption":"Andrea Dovizioso"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Editoria"
	            },
	            {
	               "name":"Libri"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Musica"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14823,
	         "title":"#AmazonPublishing e #AmazonCrossing: tante offerte in anteprima in vista del Prime Day e 8 nuovi titoli per l’estate",
	         "summary":"",
	         "publishDate":"2017-07-03T10:00:00",
	         "createDate":"2017-07-03T10:03:00",
	         "publishedBy":"",
	         "link":"http://www.ipresslive.it/comunicates/14823/amazonpublishing-e-amazoncrossing-tante-offerte-in-anteprima-in-vista-del-prime-day-e-8-nuovi-titoli-per-lestate",
	         "shortlink":"http://iprs.es/c/14823",
	         "content":null,
	         "defaultImage":{
	            "id":41483,
	            "size":194800,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20177/932939a3-c2c7-484a-a3d9-e24dbf12ec1b__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20177/932939a3-c2c7-484a-a3d9-e24dbf12ec1b__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20177/932939a3-c2c7-484a-a3d9-e24dbf12ec1b__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20177/932939a3-c2c7-484a-a3d9-e24dbf12ec1b__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20177/932939a3-c2c7-484a-a3d9-e24dbf12ec1b__O.jpg",
	            "caption":"Blog Tour Programma "
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Editoria"
	            },
	            {
	               "name":"Libri"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14778,
	         "title":"Amazon celebra Luigi Pirandello attraverso la voce di Isabella Ferrari nella Valle dei Templi di Agrigento",
	         "summary":"Per celebrare i 150 anni dalla nascita del Premio Nobel originario di Agrigento, Amazon ha organizzato mercoledì 28 giugno, all’ora del tramonto, una lettura di parti delle sue opere con i Kindle Paperwhite.\r\nA ridare vita alle parole del drammaturgo è stata la voce dell'attrice Isabella Ferrari. ",
	         "publishDate":"2017-06-29T18:00:00",
	         "createDate":"2017-06-20T18:35:00",
	         "publishedBy":"Marco Ferrario per Amazon.it",
	         "link":"http://www.ipresslive.it/comunicates/14778/amazon-celebra-luigi-pirandello-attraverso-la-voce-di-isabella-ferrari-nella-valle-dei-templi-di-agrigento",
	         "shortlink":"http://iprs.es/c/14778",
	         "content":null,
	         "defaultImage":{
	            "id":41450,
	            "size":3016651,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20176/ffded7b8-ba53-4a00-a9d1-18f0edddd42f__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20176/ffded7b8-ba53-4a00-a9d1-18f0edddd42f__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20176/ffded7b8-ba53-4a00-a9d1-18f0edddd42f__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20176/ffded7b8-ba53-4a00-a9d1-18f0edddd42f__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20176/ffded7b8-ba53-4a00-a9d1-18f0edddd42f__O.jpg",
	            "caption":"Immagini della sessione di lettura presso la Valle dei Templi con Isabella Ferrari alla luce dei Kindle Paperwhite"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Attualità"
	            },
	            {
	               "name":"Cultura"
	            },
	            {
	               "name":"Libri"
	            },
	            {
	               "name":"Locale"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14809,
	         "title":"Amazon annuncia il terzo Prime Day: 10 e 11 luglio trenta ore con centinaia di migliaia di promozioni",
	         "summary":"Cina, India e Messico si aggiungono ai festeggiamenti rendendo il Prime Day un grande evento globale in ben 13 Paesi.\r\nI clienti Prime potranno usufruire di 30 ore di shopping, con promozioni a partire dalle ore 18.00 del 10 luglio.\r\nDurante il Prime Day quasi il 40% delle Offerte lampo di tutto il mondo verrà da piccole imprese.\r\nPer festeggiare l’arrivo di Prime Day, il 9 luglio a Milano presso Piazza del Cannone, a partire dalle ore 20.00, si terrà una grande festa, aperta a tutti, con musica",
	         "publishDate":"2017-06-29T06:00:00",
	         "createDate":"2017-06-29T00:39:00",
	         "publishedBy":"Marco Ferrario per Amazon in Italia",
	         "link":"http://www.ipresslive.it/comunicates/14809/amazon-annuncia-il-terzo-prime-day-10-e-11-luglio-trenta-ore-con-centinaia-di-migliaia-di-promozioni",
	         "shortlink":"http://iprs.es/c/14809",
	         "content":null,
	         "defaultImage":{
	            "id":41443,
	            "size":624690,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20176/c376f528-2180-4b09-948a-5b08410305d2__T.png",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20176/c376f528-2180-4b09-948a-5b08410305d2__S.png",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20176/c376f528-2180-4b09-948a-5b08410305d2__M.png",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20176/c376f528-2180-4b09-948a-5b08410305d2__L.png",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20176/c376f528-2180-4b09-948a-5b08410305d2__O.png",
	            "caption":"Prime Day 2017"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Costume"
	            },
	            {
	               "name":"Distribuzione"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Editoria"
	            },
	            {
	               "name":"Hobby e tempo libero"
	            },
	            {
	               "name":"Libri"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Maschile"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            },
	            {
	               "name":"Vetrine/Shopping"
	            },
	            {
	               "name":"Video"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14793,
	         "title":"Amazon.it lancia il negozio Pet con decine di migliaia di prodotti di oltre 780 brand",
	         "summary":"In occasione dell’apertura del nuovo Negozio Animali domestici, Amazon.it invita i propri clienti a partecipare alla selezione fotografica Amazon Pet Star per avere l'opportunità di trasformare il proprio animale nel nuovo testimonial ufficiale del negozio Animali domestici Amazon. ",
	         "publishDate":"2017-06-27T08:00:00",
	         "createDate":"2017-06-27T08:34:00",
	         "publishedBy":"Marco Ferrario e Irene Artemagni per Amazon",
	         "link":"http://www.ipresslive.it/comunicates/14793/amazonit-lancia-il-negozio-pet-con-decine-di-migliaia-di-prodotti-di-oltre-780-brand",
	         "shortlink":"http://iprs.es/c/14793",
	         "content":null,
	         "defaultImage":{
	            "id":41393,
	            "size":214625,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20176/9ec6ddfc-8aae-43d3-bc49-d5dbe1cdd865__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20176/9ec6ddfc-8aae-43d3-bc49-d5dbe1cdd865__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20176/9ec6ddfc-8aae-43d3-bc49-d5dbe1cdd865__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20176/9ec6ddfc-8aae-43d3-bc49-d5dbe1cdd865__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20176/9ec6ddfc-8aae-43d3-bc49-d5dbe1cdd865__O.jpg",
	            "caption":"Kai Lian: Dog Goggles impermeabili anti UV. Occhiali da sole per cane cucciolo"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Animali"
	            },
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Familiare"
	            },
	            {
	               "name":"Femminile"
	            },
	            {
	               "name":"Hobby e tempo libero"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Maschile"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            },
	            {
	               "name":"Vetrine/Shopping"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14784,
	         "title":"La top 5 delle letture preferite dei candidati sindaco di Genova, L’Aquila, Piacenza e Verona su Amazon.it",
	         "summary":"Su Amazon.it, al link www.amazon.it/CandidatiSindaco2017, è possibile scoprire i libri preferiti da Marco Bucci e Giovanni Crivello, Americo Di Benedetto e Pierluigi Biondi, Patrizia Barbieri e Paolo Rizzi, atrizia Bisinella e Federico Sboarina.",
	         "publishDate":"2017-06-23T13:00:00",
	         "createDate":"2017-06-23T11:33:00",
	         "publishedBy":"Marco Ferrario per Amazon in Italia",
	         "link":"http://www.ipresslive.it/comunicates/14784/la-top-5-delle-letture-preferite-dei-candidati-sindaco-di-genova-laquila-piacenza-e-verona-su-amazonit",
	         "shortlink":"http://iprs.es/c/14784",
	         "content":null,
	         "defaultImage":{
	            "id":41334,
	            "size":1079466,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20176/e541fdb1-6d88-498e-9406-e494405012cf__T.png",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20176/e541fdb1-6d88-498e-9406-e494405012cf__S.png",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20176/e541fdb1-6d88-498e-9406-e494405012cf__M.png",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20176/e541fdb1-6d88-498e-9406-e494405012cf__L.png",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20176/e541fdb1-6d88-498e-9406-e494405012cf__O.png",
	            "caption":"Sergio Abramo, candidato sindaco a Catanzaro"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Cultura"
	            },
	            {
	               "name":"Libri"
	            },
	            {
	               "name":"Politica"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14780,
	         "title":"Estate 2017: #foodlovers, i migliori gadget disponibili su Amazon.it",
	         "summary":"L'appetito non va mai in vacanza, ma in viilleggiatura si veste di nuove forme e colori.",
	         "publishDate":"2017-06-21T13:00:00",
	         "createDate":"2017-06-21T13:23:00",
	         "publishedBy":"Irene Artemagni per Amazon.it",
	         "link":"http://www.ipresslive.it/comunicates/14780/estate-2017-foodlovers-i-migliori-gadget-disponibili-su-amazonit",
	         "shortlink":"http://iprs.es/c/14780",
	         "content":null,
	         "defaultImage":{
	            "id":41288,
	            "size":75938,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20176/4d6b3a43-2cf9-42fd-9bd3-a7691814f686__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20176/4d6b3a43-2cf9-42fd-9bd3-a7691814f686__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20176/4d6b3a43-2cf9-42fd-9bd3-a7691814f686__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20176/4d6b3a43-2cf9-42fd-9bd3-a7691814f686__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20176/4d6b3a43-2cf9-42fd-9bd3-a7691814f686__O.jpg",
	            "caption":"Desquamatore pesce in alluminio."
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Food & Beverage"
	            },
	            {
	               "name":"Vetrine/Shopping"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14740,
	         "title":"Amazon celebra la Gaming Week: una settimana di offerte esclusive per gli appassionati di videogiochi",
	         "summary":"Dal 12 al 18 giugno arriva la Gaming Week di Amazon, una settimana di sconti e iniziative speciali dedicate al mondo del gaming con oltre 200 offerte su prodotti Prime e di venditori terzi",
	         "publishDate":"2017-06-12T16:00:00",
	         "createDate":"2017-06-12T16:34:00",
	         "publishedBy":"Marco Ferrario per Amazon.it",
	         "link":"http://www.ipresslive.it/comunicates/14740/amazon-celebra-la-gaming-week-una-settimana-di-offerte-esclusive-per-gli-appassionati-di-videogiochi",
	         "shortlink":"http://iprs.es/c/14740",
	         "content":null,
	         "defaultImage":{
	            "id":41126,
	            "size":49342,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20176/80006a94-d03c-4013-8cb4-afee7d601a77__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20176/80006a94-d03c-4013-8cb4-afee7d601a77__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20176/80006a94-d03c-4013-8cb4-afee7d601a77__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20176/80006a94-d03c-4013-8cb4-afee7d601a77__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20176/80006a94-d03c-4013-8cb4-afee7d601a77__O.jpg",
	            "caption":"Amazon celebra la Gaming Week"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"App"
	            },
	            {
	               "name":"Giochi"
	            },
	            {
	               "name":"Giovani"
	            },
	            {
	               "name":"Maschile"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14678,
	         "title":"L’artigianato piemontese sbarca su Amazon",
	         "summary":"A partire da oggi, l’eccellenza manifatturiera della regione Piemonte sarà disponibile per i clienti di Amazon.it, Amazon.co.uk, Amazon.de e Amazon.fr\r\nAccessori moda e di design, creazioni artistiche e prelibatezze enogastronomiche piemontesi si aggiungono agli oltre 50.000 prodotti del negozio Made in Italy",
	         "publishDate":"2017-05-24T10:00:00",
	         "createDate":"2017-05-24T10:19:00",
	         "publishedBy":"Marco Ferrario per Amazon.it",
	         "link":"http://www.ipresslive.it/comunicates/14678/lartigianato-piemontese-sbarca-su-amazon",
	         "shortlink":"http://iprs.es/c/14678",
	         "content":null,
	         "defaultImage":{
	            "id":40749,
	            "size":6608066,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20175/0fdff862-f2cd-49ab-a3be-2a7531e99422__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20175/0fdff862-f2cd-49ab-a3be-2a7531e99422__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20175/0fdff862-f2cd-49ab-a3be-2a7531e99422__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20175/0fdff862-f2cd-49ab-a3be-2a7531e99422__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20175/0fdff862-f2cd-49ab-a3be-2a7531e99422__O.jpg",
	            "caption":"Conferenza Stampa nuovo negozio dedicatao all'eccellenza dei prodotti dell’artigianato piemontese disponibile da oggi su Amazon.it, Amazon.co.uk, Amazon.de e Amazon.fr"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Enogastronomia"
	            },
	            {
	               "name":"Familiare"
	            },
	            {
	               "name":"Food & Beverage"
	            },
	            {
	               "name":"Locale"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14648,
	         "title":"Amazon lancia i nuovi tablet Fire 7 e Fire HD 8",
	         "summary":"La nuova generazione di Fire 7, il tablet Amazon più venduto, è oggi ancora più sottile e leggera; disponibile a partire da €54,99. Il nuovo Fire HD 8, offre uno stupendo schermo da 8” HD con oltre 1 milione di pixel, fino a 12 ore di durata della batteria e 16GB di spazio di archiviazione, ed è sempre disponibile a partire da soli 109,99€ in offerta per i clienti Prime per un periodo limitato a partire da 89,99€.\r\n",
	         "publishDate":"2017-05-17T15:00:00",
	         "createDate":"2017-05-16T20:24:00",
	         "publishedBy":"Marco Ferrario e Irene Artemagni per Amazon in Italia",
	         "link":"http://www.ipresslive.it/comunicates/14648/amazon-lancia-i-nuovi-tablet-fire-7-e-fire-hd-8",
	         "shortlink":"http://iprs.es/c/14648",
	         "content":null,
	         "defaultImage":{
	            "id":40593,
	            "size":5043683,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20175/c6d509a2-4738-41de-8751-54d907633d1f__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20175/c6d509a2-4738-41de-8751-54d907633d1f__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20175/c6d509a2-4738-41de-8751-54d907633d1f__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20175/c6d509a2-4738-41de-8751-54d907633d1f__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20175/c6d509a2-4738-41de-8751-54d907633d1f__O.jpg",
	            "caption":"Nuovo Fire 7"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Consumatori"
	            },
	            {
	               "name":"Elettronica"
	            },
	            {
	               "name":"Giovani"
	            },
	            {
	               "name":"Hobby e tempo libero"
	            },
	            {
	               "name":"Lifestyle"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            },
	            {
	               "name":"Tecnologia (Prodotto)"
	            },
	            {
	               "name":"Telecomunicazioni"
	            },
	            {
	               "name":"Video"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14629,
	         "title":"L’Eurovision come non l’avete mai visto: Prime Now porta i propri clienti a Divano Rolling",
	         "summary":"A partire da oggi pomeriggio, giovedì 11 maggio, Amazon Prime Now metterà a disposizione dei propri clienti la possibilità di partecipare alla speciale edizione di Divano Rolling dedicata all’Eurovision.\r\nI clienti potranno vedere e commentare il programma TV assieme ad alcuni influencer d’eccezione nella cornice di Presso Milano, in via Paolo Sarpi.",
	         "publishDate":"2017-05-11T10:00:00",
	         "createDate":"2017-05-11T10:38:00",
	         "publishedBy":"Irene Artemagni per Amazon.it",
	         "link":"http://www.ipresslive.it/comunicates/14629/leurovision-come-non-lavete-mai-visto-prime-now-porta-i-propri-clienti-a-divano-rolling",
	         "shortlink":"http://iprs.es/c/14629",
	         "content":null,
	         "defaultImage":{
	            "id":40531,
	            "size":544366,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20175/7dd48251-98d8-490f-bab3-4da913a9ae76__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20175/7dd48251-98d8-490f-bab3-4da913a9ae76__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20175/7dd48251-98d8-490f-bab3-4da913a9ae76__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20175/7dd48251-98d8-490f-bab3-4da913a9ae76__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20175/7dd48251-98d8-490f-bab3-4da913a9ae76__O.jpg",
	            "caption":"L’Eurovision come non l’avete mai visto:\nPrime Now porta i propri clienti a Divano Rolling\n"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Fiere ed Eventi"
	            },
	            {
	               "name":"Giovani"
	            },
	            {
	               "name":"Hobby e tempo libero"
	            },
	            {
	               "name":"Musica"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      },
	      {
	         "id":14625,
	         "title":"Amazon Pay partecipa a Netcomm Forum ",
	         "summary":"Amazon Pay sarà presente al Netcomm Forum con lo stand presso Pad1 F1 di MiCo e con un workshop dal titolo: Amazon Pay - Semplifica l’esperienza d’acquisto per i tuoi clienti.\r\nIl workshop si terrà il 10 maggio, dalle 12.30 alle 13.00 presso la Sala Gialla 2.\r\n",
	         "publishDate":"2017-05-09T18:00:00",
	         "createDate":"2017-05-09T18:58:00",
	         "publishedBy":"Marco Ferrario per Amazon in Italia",
	         "link":"http://www.ipresslive.it/comunicates/14625/amazon-pay-partecipa-a-netcomm-forum",
	         "shortlink":"http://iprs.es/c/14625",
	         "content":null,
	         "defaultImage":{
	            "id":40508,
	            "size":568858,
	            "default":true,
	            "xsmall":"https://s3.amazonaws.com/iprs/files/images/20175/84909c7b-c123-4dc6-8a3d-1b394c8a4315__T.jpg",
	            "small":"https://s3.amazonaws.com/iprs/files/images/20175/84909c7b-c123-4dc6-8a3d-1b394c8a4315__S.jpg",
	            "medium":"https://s3.amazonaws.com/iprs/files/images/20175/84909c7b-c123-4dc6-8a3d-1b394c8a4315__M.jpg",
	            "large":"https://s3.amazonaws.com/iprs/files/images/20175/84909c7b-c123-4dc6-8a3d-1b394c8a4315__L.jpg",
	            "link":"https://s3.amazonaws.com/iprs/files/images/20175/84909c7b-c123-4dc6-8a3d-1b394c8a4315__O.jpg",
	            "caption":"Giulio Montemagno, General Manager EU Amazon Pay"
	         },
	         "images":null,
	         "attachments":null,
	         "categories":[
	            {
	               "name":"Comunicazione"
	            },
	            {
	               "name":"Consumatori"
	            },
	            {
	               "name":"Distribuzione"
	            },
	            {
	               "name":"Ecommerce"
	            },
	            {
	               "name":"Economia"
	            },
	            {
	               "name":"Tecnologia (Corporate)"
	            }
	         ],
	         "tags":null,
	         "lang":"it"
	      }
		]
	}

Get press release
*****************
Ottieni un elemento "press release"

..  http:example:: curl wget httpie python-requests

    GET /v2/pressreleases/<id> HTTP/1.1
    Host: api.ipresslive.com
    Accept: application/json

Parametri query string
Utilizziamo i parametri query string per filtrare e paginare i risultati della chiamata API. 
Il formato per i parametri query string è l'URL completo della risorsa seguito da un punto interrogativo per i parametri facoltativi:

=========   ===============   =========   =======   ================================
Param       Type (length)     Required    Default   Description
=========   ===============   =========   =======   ================================
id  		int               True		            Codice identificativo dell'elemento
=========   ===============   =========   =======   ================================


Risposta

.. code-block:: json

 	{
	   "id":25023,
	   "title":"In Italia gli acquisti digitali per Turismo e Viaggi valgono 11,2 miliardi di €, il 20% del mercato Travel complessivo",
	   "summary":"Cresce il valore della componente digitale sul mercato italiano, \r\nche comprende anche la spesa dei turisti stranieri, oltrepassando un quinto del totale (+9% nel 2017 mentre nel 2016 cresceva dell’8%).\r\nIl mondo dei Trasporti raccoglie il 73% del mercato (con un incremento del valore pari all’8%), seguito dalle Strutture ricettive con il 15% (+10%) e dai Pacchetti viaggio con il 12% (+15%).\r\n\r\nRimane costante l’incidenza del transato derivante dai canali indiretti sul totale del mercato digital",
	   "publishDate":"2017-10-12T15:00:00",
	   "createDate":"2017-10-12T15:32:00",
	   "publishedBy":"Marco Ferrario e Daniele Gatti per Politecnico di Milano",
	   "link":"http://www.ipresslive.it/comunicates/25023/in-italia-gli-acquisti-digitali-per-turismo-e-viaggi-valgono-112-miliardi-di-il-20-del-mercato-travel-complessivo",
	   "shortlink":"http://iprs.es/c/25023",
	   "content":"<p>Full html content..........</p>",
	   "defaultImage":{
	      "id":53886,
	      "size":121533,
	      "default":true,
	      "xsmall":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__T.png",
	      "small":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__S.png",
	      "medium":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__M.png",
	      "large":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__L.png",
	      "link":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__O.png",
	      "caption":"Il mercato del Turismo nel 2017 in Italia ."
	   },
	   "images":[
	      {
	         "id":53886,
	         "size":121533,
	         "default":false,
	         "xsmall":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__T.png",
	         "small":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__S.png",
	         "medium":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__M.png",
	         "large":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__L.png",
	         "link":"https://s3.amazonaws.com/iprs/files/images/201710/ff6a3c53-8d1b-4e13-a8da-8044e487eeb9__O.png",
	         "caption":"Il mercato del Turismo nel 2017 in Italia ."
	      },
	      {
	         "id":53891,
	         "size":119614,
	         "default":false,
	         "xsmall":"https://s3.amazonaws.com/iprs/files/images/201710/2535ee10-aef4-457f-a450-1885a0dc6982__T.png",
	         "small":"https://s3.amazonaws.com/iprs/files/images/201710/2535ee10-aef4-457f-a450-1885a0dc6982__S.png",
	         "medium":"https://s3.amazonaws.com/iprs/files/images/201710/2535ee10-aef4-457f-a450-1885a0dc6982__M.png",
	         "large":"https://s3.amazonaws.com/iprs/files/images/201710/2535ee10-aef4-457f-a450-1885a0dc6982__L.png",
	         "link":"https://s3.amazonaws.com/iprs/files/images/201710/2535ee10-aef4-457f-a450-1885a0dc6982__O.png",
	         "caption":"Tasporti, alloggi e mobile commerce nel Turismo 2017."
	      },
	      {
	         "id":53887,
	         "size":200798,
	         "default":false,
	         "xsmall":"https://s3.amazonaws.com/iprs/files/images/201710/a5d50419-9589-4e42-a994-9090094e6f8e__T.png",
	         "small":"https://s3.amazonaws.com/iprs/files/images/201710/a5d50419-9589-4e42-a994-9090094e6f8e__S.png",
	         "medium":"https://s3.amazonaws.com/iprs/files/images/201710/a5d50419-9589-4e42-a994-9090094e6f8e__M.png",
	         "large":"https://s3.amazonaws.com/iprs/files/images/201710/a5d50419-9589-4e42-a994-9090094e6f8e__L.png",
	         "link":"https://s3.amazonaws.com/iprs/files/images/201710/a5d50419-9589-4e42-a994-9090094e6f8e__O.png",
	         "caption":"Il turista digitale fa zapping tra canali fisici e digitali."
	      },
	      {
	         "id":53889,
	         "size":204317,
	         "default":false,
	         "xsmall":"https://s3.amazonaws.com/iprs/files/images/201710/14c49e14-ba6b-42c6-a959-72ba8e4d688e__T.png",
	         "small":"https://s3.amazonaws.com/iprs/files/images/201710/14c49e14-ba6b-42c6-a959-72ba8e4d688e__S.png",
	         "medium":"https://s3.amazonaws.com/iprs/files/images/201710/14c49e14-ba6b-42c6-a959-72ba8e4d688e__M.png",
	         "large":"https://s3.amazonaws.com/iprs/files/images/201710/14c49e14-ba6b-42c6-a959-72ba8e4d688e__L.png",
	         "link":"https://s3.amazonaws.com/iprs/files/images/201710/14c49e14-ba6b-42c6-a959-72ba8e4d688e__O.png",
	         "caption":"I diversi gruppi dei turisti digitali."
	      },
	      {
	         "id":53888,
	         "size":174333,
	         "default":false,
	         "xsmall":"https://s3.amazonaws.com/iprs/files/images/201710/21a86d93-5c5e-4c8e-9281-ab759515464a__T.png",
	         "small":"https://s3.amazonaws.com/iprs/files/images/201710/21a86d93-5c5e-4c8e-9281-ab759515464a__S.png",
	         "medium":"https://s3.amazonaws.com/iprs/files/images/201710/21a86d93-5c5e-4c8e-9281-ab759515464a__M.png",
	         "large":"https://s3.amazonaws.com/iprs/files/images/201710/21a86d93-5c5e-4c8e-9281-ab759515464a__L.png",
	         "link":"https://s3.amazonaws.com/iprs/files/images/201710/21a86d93-5c5e-4c8e-9281-ab759515464a__O.png",
	         "caption":"Le innovazioni digitali nella agenzie di viaggio."
	      },
	      {
	         "id":53890,
	         "size":247083,
	         "default":false,
	         "xsmall":"https://s3.amazonaws.com/iprs/files/images/201710/e2828f32-100f-412b-a507-cfa4551bcfb3__T.png",
	         "small":"https://s3.amazonaws.com/iprs/files/images/201710/e2828f32-100f-412b-a507-cfa4551bcfb3__S.png",
	         "medium":"https://s3.amazonaws.com/iprs/files/images/201710/e2828f32-100f-412b-a507-cfa4551bcfb3__M.png",
	         "large":"https://s3.amazonaws.com/iprs/files/images/201710/e2828f32-100f-412b-a507-cfa4551bcfb3__L.png",
	         "link":"https://s3.amazonaws.com/iprs/files/images/201710/e2828f32-100f-412b-a507-cfa4551bcfb3__O.png",
	         "caption":"La provenienza delle prenotazioni nelle strutture ricettive e nella ristorazione."
	      }
	   ],
	   "attachments":[
	      {
	         "id":53884,
	         "size":423958,
	         "caption":"Comunicato in pdf",
	         "link":"https://s3.amazonaws.com/iprs/files/attachments/201710/c5544951-771f-40e6-9b12-0a91056fba58__O.pdf"
	      }
	   ],
	   "categories":[
	      {
	         "name":"Comunicazione"
	      },
	      {
	         "name":"Economia"
	      },
	      {
	         "name":"Tecnologia (Corporate)"
	      },
	      {
	         "name":"Turismo"
	      }
	   ],
	   "tags":null,
	   "lang":"it"
	}

