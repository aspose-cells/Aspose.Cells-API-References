---
title: "Classe WebQueryConnection"
linktitle: "WebQueryConnection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe WebQueryConnection. Incapsula l'oggetto che rappresenta webqueryconnection in Go."
type: docs
weight: 200
url: /it/go-cpp/webqueryconnection/
---

## WebQueryConnection class

Specifica le proprietà per una sorgente di query web. Una query web recupera dati dalle tabelle HTML e può anche fornire parametri HTTP "Get" da elaborare dal server web nella generazione dell'HTML includendo i parametri e gli elementi dei parametri.

```go

type WebQueryConnection struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewWebQueryConnection](./newwebqueryconnection/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetClassType](./getclasstype/) | Restituisce il tipo di questo oggetto ExternalConnection. |
| [IsXml](./isxml/) | true se la sorgente della query web è XML (anziché HTML), altrimenti false. |
| [SetIsXml](./setisxml/) | true se la sorgente della query web è XML (anziché HTML), altrimenti false. |
| [IsXl97](./isxl97/) | Questo flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostato su true se questa query web è stata creata in Microsoft Excel 97. Questo è un attributo opzionale che può essere ignorato. |
| [SetIsXl97](./setisxl97/) | Questo flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostato su true se questa query web è stata creata in Microsoft Excel 97. Questo è un attributo opzionale che può essere ignorato. |
| [IsXl2000](./isxl2000/) | Questo flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostato su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. Questo è un attributo opzionale che può essere ignorato. |
| [SetIsXl2000](./setisxl2000/) | Questo flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostato su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. Questo è un attributo opzionale che può essere ignorato. |
| [GetUrl](./geturl/) | URL da utilizzare per aggiornare i dati esterni. |
| [SetUrl](./seturl/) | URL da utilizzare per aggiornare i dati esterni. |
| [GetConnectionFile](./getconnectionfile/) | Restituisce il file di connessione. |
| [IsTextDates](./istextdates/) | Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date. |
| [SetIsTextDates](./setistextdates/) | Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date. |
| [IsXmlSourceData](./isxmlsourcedata/) | Flag che indica che i dati sorgente XML devono essere importati al posto della tabella HTML stessa. |
| [SetIsXmlSourceData](./setisxmlsourcedata/) | Flag che indica che i dati sorgente XML devono essere importati al posto della tabella HTML stessa. |
| [GetPost](./getpost/) | Restituisce o imposta la stringa utilizzata con il metodo POST per inserire dati in un server web per restituire dati da una query web. |
| [SetPost](./setpost/) | Restituisce o imposta la stringa utilizzata con il metodo POST per inserire dati in un server web per restituire dati da una query web. |
| [IsParsePre](./isparsepre/) | Flag che indica se i dati contenuti nei tag HTML PRE nella pagina web vengono analizzati in colonne quando si importa la pagina in una tabella di query. |
| [SetIsParsePre](./setisparsepre/) | Flag che indica se i dati contenuti nei tag HTML PRE nella pagina web vengono analizzati in colonne quando si importa la pagina in una tabella di query. |
| [IsHtmlTables](./ishtmltables/) | Flag che indica se le query web devono funzionare solo su tabelle HTML. |
| [SetIsHtmlTables](./setishtmltables/) | Flag che indica se le query web devono funzionare solo su tabelle HTML. |
| [GetHtmlFormat](./gethtmlformat/) | Come gestire la formattazione dalla sorgente HTML quando si trasferiscono i dati della query web nel foglio di lavoro. Rilevante quando sourceData è True. |
| [SetHtmlFormat](./sethtmlformat/) | Come gestire la formattazione dalla sorgente HTML quando si trasferiscono i dati della query web nel foglio di lavoro. Rilevante quando sourceData è True. |
| [IsSameSettings](./issamesettings/) | Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga. |
| [SetIsSameSettings](./setissamesettings/) | Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga. |
| [GetEditWebPage](./geteditwebpage/) | L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL viene conservato nel caso in cui sourceData="true" e l'url sia stato reindirizzato a un file XML. In tal modo la pagina destinata all'utente può essere mostrata nell'interfaccia utente e i dati XML possono essere recuperati in background. |
| [SetEditWebPage](./seteditwebpage/) | L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL viene conservato nel caso in cui sourceData="true" e l'url sia stato reindirizzato a un file XML. In tal modo la pagina destinata all'utente può essere mostrata nell'interfaccia utente e i dati XML possono essere recuperati in background. |
| [IsConsecutive](./isconsecutive/) | Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore. |
| [SetIsConsecutive](./setisconsecutive/) | Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore. |
| [GetId](./getid/) | Restituisce l'ID della connessione. |
| [GetSourceType](./getsourcetype/) | Restituisce o imposta il tipo DataSource della connessione esterna. |
| [SetSourceType](./setsourcetype/) | Restituisce o imposta il tipo DataSource della connessione esterna. |
| [GetSSOId](./getssoid/) | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server intermediatespreadsheetML e la fonte dati esterna. |
| [SetSSOId](./setssoid/) | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server intermediatespreadsheetML e la fonte dati esterna. |
| [GetSavePassword](./getsavepassword/) | True se la password deve essere salvata come parte della stringa di connessione; altrimenti, False. |
| [SetSavePassword](./setsavepassword/) | True se la password deve essere salvata come parte della stringa di connessione; altrimenti, False. |
| [GetSaveData](./getsavedata/) | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, false. |
| [SetSaveData](./setsavedata/) | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, false. |
| [GetRefreshOnLoad](./getrefreshonload/) | True se questa connessione deve essere aggiornata all'apertura del file; altrimenti, false. |
| [SetRefreshOnLoad](./setrefreshonload/) | True se questa connessione deve essere aggiornata all'apertura del file; altrimenti, false. |
| [GetReconnectionMethodType](./getreconnectionmethodtype/) | Specifica cosa deve fare l'applicazione di foglio elettronico quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required. |
| [SetReconnectionMethodType](./setreconnectionmethodtype/) | Specifica cosa deve fare l'applicazione di foglio elettronico quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required. |
| [GetOnlyUseConnectionFile](./getonlyuseconnectionfile/) | Indica se l'applicazione di foglio elettronico deve sempre e solo utilizzare le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione di foglio elettronico deve seguire la procedura indicata dall'attributo reconnectionMethod. |
| [SetOnlyUseConnectionFile](./setonlyuseconnectionfile/) | Indica se l'applicazione di foglio elettronico deve sempre e solo utilizzare le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione di foglio elettronico deve seguire la procedura indicata dall'attributo reconnectionMethod. |
| [GetOdcFile](./getodcfile/) | Specifica il percorso completo al file di connessione esterno da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati, e reconnectionMethod=1, l'applicazione di foglio elettronico proverà di nuovo utilizzando le informazioni dal file di connessione esterno invece dell'oggetto di connessione incorporato nella cartella di lavoro. |
| [SetOdcFile](./setodcfile/) | Specifica il percorso completo al file di connessione esterno da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati, e reconnectionMethod=1, l'applicazione di foglio elettronico proverà di nuovo utilizzando le informazioni dal file di connessione esterno invece dell'oggetto di connessione incorporato nella cartella di lavoro. |
| [GetSourceFile](./getsourcefile/) | Utilizzato quando la fonte dati esterna è basata su file. Quando una connessione a tale fonte dati fallisce, l'applicazione di foglio elettronico tenta di connettersi direttamente a questo file. Può essere espresso in URI o notazione di percorso file specifica del sistema. |
| [SetSourceFile](./setsourcefile/) | Utilizzato quando la fonte dati esterna è basata su file. Quando una connessione a tale fonte dati fallisce, l'applicazione di foglio elettronico tenta di connettersi direttamente a questo file. Può essere espresso in URI o notazione di percorso file specifica del sistema. |
| [IsNew](./isnew/) | True se la connessione non è stata aggiornata per la prima volta; altrimenti, false. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno dei risultati. |
| [SetIsNew](./setisnew/) | True se la connessione non è stata aggiornata per la prima volta; altrimenti, false. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno dei risultati. |
| [GetName](./getname/) | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco. |
| [SetName](./setname/) | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco. |
| [GetKeepAlive](./getkeepalive/) | True quando l'applicazione di foglio elettronico deve fare sforzi per mantenere la connessione aperta. Quando false, l'applicazione deve chiudere la connessione dopo aver recuperato le informazioni. |
| [SetKeepAlive](./setkeepalive/) | True quando l'applicazione di foglio elettronico deve fare sforzi per mantenere la connessione aperta. Quando false, l'applicazione deve chiudere la connessione dopo aver recuperato le informazioni. |
| [GetRefreshInternal](./getrefreshinternal/) | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione. |
| [SetRefreshInternal](./setrefreshinternal/) | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione. |
| [GetConnectionDescription](./getconnectiondescription/) | Specifica la descrizione dell'utente per questa connessione |
| [SetConnectionDescription](./setconnectiondescription/) | Specifica la descrizione dell'utente per questa connessione |
| [IsDeleted](./isdeleted/) | Indica se la connessione del workbook associata è stata eliminata. true se la connessione è stata eliminata; altrimenti, false. |
| [SetIsDeleted](./setisdeleted/) | Indica se la connessione del workbook associata è stata eliminata. true se la connessione è stata eliminata; altrimenti, false. |
| [GetCredentialsMethodType](./getcredentialsmethodtype/) | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione. |
| [SetCredentialsMethodType](./setcredentialsmethodtype/) | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione. |
| [GetBackgroundRefresh](./getbackgroundrefresh/) | Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronamente in background; false se l'uso preferito della connessione è aggiornare sincronicamente in primo piano. |
| [SetBackgroundRefresh](./setbackgroundrefresh/) | Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronamente in background; false se l'uso preferito della connessione è aggiornare sincronicamente in primo piano. |
| [GetParameters](./getparameters/) | Ottiene ConnectionParameterCollection per una query ODBC o web. |
| [GetPowerQueryFormula](./getpowerqueryformula/) | Ottiene la definizione della formula power query. |
| [GetCommand](./getcommand/) | La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati |
| [SetCommand](./setcommand/) | La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati |
| [GetCommandType](./getcommandtype/) | Specifica il tipo di comando OLE DB. 1. Query specifica un nome di cubo 2. Query specifica un'istruzione SQL 3. Query specifica un nome di tabella 4. Query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. Query è contro un List Data Provider basato sul web. |
| [SetCommandType](./setcommandtype/) | Specifica il tipo di comando OLE DB. 1. Query specifica un nome di cubo 2. Query specifica un'istruzione SQL 3. Query specifica un nome di tabella 4. Query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. Query è contro un List Data Provider basato sul web. |
| [GetConnectionString](./getconnectionstring/) | La stringa di informazioni di connessione è usata per stabilire un contatto con una fonte dati OLE DB o ODBC. |
| [SetConnectionString](./setconnectionstring/) | La stringa di informazioni di connessione è usata per stabilire un contatto con una fonte dati OLE DB o ODBC. |
| [GetSecondCommand](./getsecondcommand/) | Specifica una seconda stringa di testo del comando che viene conservata quando i campi di pagina basati su server di PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (non è presente clausola WHERE nella prima). In base a questi 2 comandi (Command e ServerCommand), l'interfaccia utente dei parametri può essere popolata e possono essere costruite query parametrizzate. |
| [SetSecondCommand](./setsecondcommand/) | Specifica una seconda stringa di testo del comando che viene conservata quando i campi di pagina basati su server di PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (non è presente clausola WHERE nella prima). In base a questi 2 comandi (Command e ServerCommand), l'interfaccia utente dei parametri può essere popolata e possono essere costruite query parametrizzate. |
