---
title: classe WebQueryConnection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---
##  classe WebQueryConnection
 Specifica le proprietà per un'origine di query Web. Una query Web recupererà i dati dalle tabelle HTML,
 e può anche fornire parametri HTTP "Get" che devono essere elaborati dal web server nella generazione dello HTML da parte di
compresi i parametri e gli elementi dei parametri.



**Eredità:** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)



Il tipo WebQueryConnection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [id](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/id) | Ottiene l'ID della connessione.|
| [power_query_formula](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) | Ottiene la definizione della formula di query di alimentazione.|
| [type](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/type) | Ottiene o imposta il tipo DataSource della connessione esterna.|
| [source_file](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) | Utilizzato quando l'origine dati esterna è basata su file. Quando una connessione a tali dati<br/> source non riesce, l'applicazione del foglio di calcolo tenta di connettersi direttamente a questo file. Forse<br/> espresso in URI o notazione del percorso file specifica del sistema.|
| [sso_id](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un intermediario<br/> server spreadsheetML e l'origine dati esterna.|
| [save_password](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) | True se la password deve essere salvata come parte della stringa di connessione; altrimenti Falso.|
| [save_data](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati<br/> con la cartella di lavoro; altrimenti, falso.|
| [refresh_on_load](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) | True se questa connessione deve essere aggiornata all'apertura del file; altrimenti, falso.|
| [reconnection_method_type](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) | Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione fallisce.<br/>Il valore predefinito è ReConnectionMethodType.Required.|
| [reconnection_method](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) | Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione fallisce.<br/>Il valore predefinito è ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) | Indica se l'applicazione per fogli di calcolo deve utilizzare sempre e solo il file<br/> informazioni sulla connessione nel file di connessione esterno indicato dall'attributo odcFile<br/> quando la connessione viene aggiornata. Se falso, l'applicazione del foglio di calcolo<br/> deve seguire la procedura indicata dall'attributo reconnectionMethod|
| [odc_file](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) | Specifica il percorso completo del file di connessione esterno da cui proveniva questa connessione<br/> creato. Se una connessione non riesce durante un tentativo di aggiornamento dei dati e reconnectionMethod=1,<br/> quindi l'applicazione del foglio di calcolo riproverà utilizzando le informazioni dal file di connessione esterno<br/> invece dell'oggetto connessione incorporato nella cartella di lavoro.|
| [is_new](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) | True se la connessione non è stata aggiornata per la prima volta; altrimenti, falso.<br/> Questo stato può verificarsi quando l'utente salva il file prima che sia terminata la restituzione di una query.|
| [name](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/name) | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco.|
| [keep_alive](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) | Vero quando l'applicazione del foglio di calcolo deve sforzarsi di mantenere la connessione<br/>aprire. Se falso, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato il file<br/> informazione.|
| [refresh_internal](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione.|
| [connection_id](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) | Specifica l'identificatore univoco di questa connessione.|
| [connection_description](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) | Specifica la descrizione utente per questa connessione|
| [is_deleted](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) |Indica se la connessione alla cartella di lavoro associata è stata eliminata. vero se il<br/> la connessione è stata cancellata; altrimenti, falso.|
| [credentials_method_type](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione.|
| [credentials](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione.|
| [background_refresh](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) | Indica se la connessione può essere aggiornata in background (in modo asincrono).<br/>true se l'utilizzo preferito della connessione consiste nell'aggiornare in modo asincrono in background;<br/> false se l'utilizzo preferito della connessione consiste nell'aggiornare in modo sincrono in primo piano.|
| [parameters](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) | Ottiene [ConnectionParameterCollection](/cells/it/python-net/aspose.cells.externalconnections/connectionparametercollection) per una query ODBC o Web.|
| [is_xml](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) | true se l'origine della query Web è XML (invece di HTML), altrimenti false.|
| [is_xl97](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) |Questo flag esiste per la retrocompatibilità con i file di fogli di calcolo esistenti meno recenti ed è impostato<br/>su true se questa query Web è stata creata in Microsoft Excel 97.<br/> Questo è un attributo facoltativo che può essere ignorato.|
| [is_xl2000](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) |Questo flag esiste per la retrocompatibilità con i file di fogli di calcolo esistenti meno recenti ed è impostato<br/>su true se questa query Web è stata aggiornata in un'applicazione per fogli di calcolo più recente o uguale<br/>al numero Microsoft Excel 2000.<br/> Questo è un attributo facoltativo che può essere ignorato.|
| [url](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/url) | URL da utilizzare per aggiornare i dati esterni.|
| [is_text_dates](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) | Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date.|
| [is_xml_source_data](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) | Flag che indica che i dati di origine XML devono essere importati anziché la tabella HTML stessa.|
| [post](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/post) | Restituisce o imposta la stringa utilizzata con il metodo post per inserire i dati in un server web<br/> per restituire dati da una query web.|
| [is_parse_pre](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) | Flag che indica se i dati contenuti all'interno dei tag HTML PRE nella pagina web sono<br/> analizzato in colonne quando si importa la pagina in una tabella di query.|
| [is_html_tables](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) | Flag che indica se le query Web devono funzionare solo sulle tabelle HTML.|
| [html_format](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) | Come gestire la formattazione dall'origine HTML quando si portano i dati delle query web nel file<br/> foglio di lavoro. Rilevante quando sourceData è True.|
| [is_same_settings](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) |Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza<br/> come prima fila.|
| [edit_web_page](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) | L'URL della pagina web rivolta all'utente che mostra i dati della query web. Questo URL è persistente<br/>nel caso in cui sourceData="true" e url siano stati reindirizzati per fare riferimento a un file XML.<br/>Quindi la pagina rivolta all'utente può essere visualizzata nell'interfaccia utente e i dati XML possono essere recuperati<br/> dietro le quinte.|
| [edit_page](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) | L'URL della pagina web rivolta all'utente che mostra i dati della query web. Questo URL è persistente<br/>nel caso in cui sourceData="true" e url siano stati reindirizzati per fare riferimento a un file XML.<br/>Quindi la pagina rivolta all'utente può essere visualizzata nell'interfaccia utente e i dati XML possono essere recuperati<br/> dietro le quinte.|
| [is_consecutive](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) | Flag che indica se i delimitatori consecutivi devono essere trattati come un solo delimitatore.|



###  Guarda anche
* modulo [aspose.cells.externalconnections](..)
* classe [ConnectionParameterCollection](/cells/it/python-net/aspose.cells.externalconnections/connectionparametercollection)
* classe [ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)
* classe [WebQueryConnection](/cells/it/python-net/aspose.cells.externalconnections/webqueryconnection)
