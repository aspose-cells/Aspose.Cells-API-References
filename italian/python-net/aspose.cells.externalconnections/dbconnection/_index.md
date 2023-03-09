---
title: classe DBConnection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells.externalconnections/dbconnection/
is_root: false
---
##  classe DBConnection
Specifica tutte le proprietà associate a una connessione dati esterna ODBC o OLE DB.



**Eredità:** [DBConnection](/cells/python-net/aspose.cells.externalconnections/dbconnection) → 
[ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)



Il tipo DBConnection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [id](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/id) | Ottiene l'id della connessione.|
| [power_query_formula](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/power_query_formula) | Ottiene la definizione della formula di query di alimentazione.|
| [type](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/type) | Ottiene o imposta il tipo DataSource della connessione esterna.|
| [source_file](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/source_file) | Utilizzato quando l'origine dati esterna è basata su file.<br/> source non riesce, l'applicazione del foglio di calcolo tenta di connettersi direttamente a questo file.<br/> espresso in URI o notazione del percorso file specifica del sistema.|
| [sso_id](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/sso_id) | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un intermediario<br/> server spreadsheetML e l'origine dati esterna.|
| [save_password](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/save_password) | True se la password deve essere salvata come parte della stringa di connessione; in caso contrario, False.|
| [save_data](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/save_data) | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati<br/> con la cartella di lavoro; in caso contrario, false.|
| [refresh_on_load](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/refresh_on_load) | True se questa connessione deve essere aggiornata all'apertura del file;|
| [reconnection_method_type](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method_type) | Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione fallisce.<br/>Il valore predefinito è ReConnectionMethodType.Required.|
| [reconnection_method](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method) | Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione fallisce.<br/>Il valore predefinito è ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/only_use_connection_file) | Indica se l'applicazione per fogli di calcolo deve utilizzare sempre e solo il file<br/> informazioni sulla connessione nel file di connessione esterno indicato dall'attributo odcFile<br/> quando la connessione viene aggiornata. Se falso, l'applicazione del foglio di calcolo<br/> deve seguire la procedura indicata dall'attributo reconnectionMethod|
| [odc_file](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/odc_file) | Specifica il percorso completo del file di connessione esterno da cui proveniva questa connessione<br/> Se una connessione non riesce durante un tentativo di aggiornamento dei dati e reconnectionMethod=1,<br/> quindi l'applicazione del foglio di calcolo riproverà utilizzando le informazioni dal file di connessione esterno<br/> invece dell'oggetto connessione incorporato nella cartella di lavoro.|
| [is_new](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/is_new) | True se la connessione non è stata aggiornata per la prima volta; in caso contrario, false.<br/> Questo stato può verificarsi quando l'utente salva il file prima che sia terminata la restituzione di una query.|
| [name](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/name) | Specifica il nome della connessione.|
| [keep_alive](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/keep_alive) | Vero quando l'applicazione del foglio di calcolo deve sforzarsi di mantenere la connessione<br/>open Se falso, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato il file<br/> informazione.|
| [refresh_internal](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/refresh_internal) | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione.|
| [connection_id](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/connection_id) | Specifica l'identificatore univoco di questa connessione.|
| [connection_description](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/connection_description) | Specifica la descrizione utente per questa connessione|
| [is_deleted](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/is_deleted) |Indica se la connessione alla cartella di lavoro associata è stata eliminata true se il<br/> altrimenti, falso.|
| [credentials_method_type](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/credentials_method_type) | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione.|
| [credentials](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/credentials) | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione.|
| [background_refresh](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/background_refresh) | Indica se la connessione può essere aggiornata in background (in modo asincrono).<br/>true se l'utilizzo preferito della connessione consiste nell'aggiornare in modo asincrono in background;<br/> false se l'utilizzo preferito della connessione consiste nell'aggiornare in modo sincrono in primo piano.|
| [parameters](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/parameters) | Ottiene [ConnectionParameterCollection](/cells/it/python-net/aspose.cells.externalconnections/connectionparametercollection) per una query ODBC o Web.|
| [connection_info](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/connection_info) | La stringa delle informazioni di connessione viene utilizzata per stabilire un contatto con un'origine dati OLE DB o ODBC.|
| [command_type](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/command_type) | Specifica il tipo di comando OLE DB.<br/>1. La query specifica il nome di un cubo<br/>2. La query specifica un'istruzione SQL<br/>3. La query specifica un nome di tabella<br/>4. La query specifica che sono state fornite informazioni predefinite e spetta al provider come interpretarle.<br/> 5. La query è rivolta a un fornitore di dati List basato sul Web.|
| [command](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/command) | La stringa contenente il comando del database da passare al fornitore di dati API che lo farà<br/> interagire con la fonte esterna per recuperare i dati|
| [sever_command](/cells/it/python-net/aspose.cells.externalconnections/dbconnection/sever_command) |Specifica una seconda stringa di testo del comando che viene mantenuta quando la tabella pivot è basata sul server<br/> i campi della pagina sono in uso.<br/> Per le connessioni ODBC, serverCommand è in genere una query più ampia rispetto a command (no<br/>La clausola WHERE è presente nella prima).<br/> l'interfaccia utente dei parametri può essere popolata e possono essere costruite query con parametri|



###  Guarda anche
* modulo [aspose.cells.externalconnections](..)
* classe [ConnectionParameterCollection](/cells/it/python-net/aspose.cells.externalconnections/connectionparametercollection)
* classe [DBConnection](/cells/it/python-net/aspose.cells.externalconnections/dbconnection)
* classe [ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)
