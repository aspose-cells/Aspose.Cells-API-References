---
title: classe DataModelConnection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.externalconnections/datamodelconnection/
is_root: false
---
##  classe DataModelConnection
Specifica una connessione al modello di dati



**Eredità:** [DataModelConnection](/cells/python-net/aspose.cells.externalconnections/datamodelconnection) → 
[ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)



Il tipo DataModelConnection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [id](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/id) | Ottiene l'id della connessione.|
| [power_query_formula](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/power_query_formula) | Ottiene la definizione della formula di query di alimentazione.|
| [type](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/type) | Ottiene o imposta il tipo DataSource della connessione esterna.|
| [source_file](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/source_file) | Utilizzato quando l'origine dati esterna è basata su file. Quando una connessione a tali dati<br/> source non riesce, l'applicazione del foglio di calcolo tenta di connettersi direttamente a questo file. Forse<br/> espresso in URI o notazione del percorso file specifica del sistema.|
| [sso_id](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/sso_id) | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un intermediario<br/>server spreadsheetML e l'origine dati esterna.|
| [save_password](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/save_password) |True se la password deve essere salvata come parte della stringa di connessione; altrimenti Falso.|
| [save_data](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/save_data) | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati<br/> con la cartella di lavoro; altrimenti, falso.|
| [refresh_on_load](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/refresh_on_load) | True se questa connessione deve essere aggiornata all'apertura del file; altrimenti, falso.|
| [reconnection_method_type](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/reconnection_method_type) | Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione fallisce.<br/> Il valore predefinito è ReConnectionMethodType.Required.|
| [reconnection_method](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/reconnection_method) | Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione fallisce.<br/> Il valore predefinito è ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/only_use_connection_file) | Indica se l'applicazione per fogli di calcolo deve utilizzare sempre e solo il file<br/> informazioni sulla connessione nel file di connessione esterno indicato dall'attributo odcFile<br/> quando la connessione viene aggiornata. Se falso, l'applicazione del foglio di calcolo<br/> deve seguire la procedura indicata dall'attributo reconnectionMethod|
| [odc_file](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/odc_file) | Specifica il percorso completo del file di connessione esterno da cui proveniva questa connessione<br/> creato. Se una connessione non riesce durante un tentativo di aggiornamento dei dati e reconnectionMethod=1,<br/> quindi l'applicazione del foglio di calcolo riproverà utilizzando le informazioni dal file di connessione esterno<br/> invece dell'oggetto connessione incorporato nella cartella di lavoro.|
| [is_new](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/is_new) | True se la connessione non è stata aggiornata per la prima volta; altrimenti, falso.<br/> Questo stato può verificarsi quando l'utente salva il file prima che sia terminata la restituzione di una query.|
| [name](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/name) | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco.|
| [keep_alive](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/keep_alive) | Vero quando l'applicazione del foglio di calcolo deve sforzarsi di mantenere la connessione<br/> aprire. Se falso, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato il file<br/> informazione.|
| [refresh_internal](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/refresh_internal) | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione.|
| [connection_id](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/connection_id) | Specifica l'identificatore univoco di questa connessione.|
| [connection_description](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/connection_description) | Specifica la descrizione utente per questa connessione|
| [is_deleted](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/is_deleted) | Indica se la connessione alla cartella di lavoro associata è stata eliminata. vero se il<br/> la connessione è stata cancellata; altrimenti, falso.|
| [credentials_method_type](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/credentials_method_type) | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione.|
| [credentials](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/credentials) | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione.|
| [background_refresh](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/background_refresh) | Indica se la connessione può essere aggiornata in background (in modo asincrono).<br/> true se l'utilizzo preferito della connessione consiste nell'aggiornare in modo asincrono in background;<br/>false se l'utilizzo preferito della connessione consiste nell'aggiornare in modo sincrono in primo piano.|
| [parameters](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection/parameters) | Ottiene [ConnectionParameterCollection](/cells/it/python-net/aspose.cells.externalconnections/connectionparametercollection) per una query ODBC o Web.|



###  Guarda anche
* modulo [aspose.cells.externalconnections](..)
* classe [ConnectionParameterCollection](/cells/it/python-net/aspose.cells.externalconnections/connectionparametercollection)
* classe [DataModelConnection](/cells/it/python-net/aspose.cells.externalconnections/datamodelconnection)
* classe [ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)
