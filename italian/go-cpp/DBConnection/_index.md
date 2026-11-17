---
title: "Classe DBConnection"
linktitle: "DBConnection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe DBConnection. Incapsula l'oggetto che rappresenta dbconnection in Go."
type: docs
weight: 200
url: /it/go-cpp/dbconnection/
---

## DBConnection class

Specifica tutte le proprietà associate a una connessione dati esterna ODBC o OLE DB.

```go

type DBConnection struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewDBConnection](./newdbconnection/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetClassType](./getclasstype/) | Restituisce il tipo di questo oggetto ExternalConnection. |
| [GetConnectionString](./getconnectionstring/) | La stringa di informazioni di connessione è usata per stabilire un contatto con una fonte dati OLE DB o ODBC. |
| [SetConnectionString](./setconnectionstring/) | La stringa di informazioni di connessione è usata per stabilire un contatto con una fonte dati OLE DB o ODBC. |
| [GetPowerQueryFormula](./getpowerqueryformula/) | Ottiene la definizione della formula power query. |
| [GetCommandType](./getcommandtype/) | Specifica il tipo di comando OLE DB. 1. Query specifica un nome di cubo 2. Query specifica un'istruzione SQL 3. Query specifica un nome di tabella 4. Query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. Query è contro un List Data Provider basato sul web. |
| [SetCommandType](./setcommandtype/) | Specifica il tipo di comando OLE DB. 1. Query specifica un nome di cubo 2. Query specifica un'istruzione SQL 3. Query specifica un nome di tabella 4. Query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. Query è contro un List Data Provider basato sul web. |
| [GetCommand](./getcommand/) | La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati |
| [SetCommand](./setcommand/) | La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati |
| [GetSecondCommand](./getsecondcommand/) | Specifica una seconda stringa di testo del comando che viene conservata quando i campi di pagina basati su server di PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (non è presente clausola WHERE nella prima). In base a questi 2 comandi (Command e ServerCommand), l'interfaccia utente dei parametri può essere popolata e possono essere costruite query parametrizzate. |
| [SetSecondCommand](./setsecondcommand/) | Specifica una seconda stringa di testo del comando che viene conservata quando i campi di pagina basati su server di PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (non è presente clausola WHERE nella prima). In base a questi 2 comandi (Command e ServerCommand), l'interfaccia utente dei parametri può essere popolata e possono essere costruite query parametrizzate. |
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
| [GetConnectionFile](./getconnectionfile/) | Restituisce il file di connessione. |
