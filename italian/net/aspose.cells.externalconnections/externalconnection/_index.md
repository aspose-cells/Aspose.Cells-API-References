---
title: ExternalConnection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Specifica una connessione dati esterna
type: docs
weight: 3290
url: /it/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Specifica una connessione dati esterna

```csharp
public abstract class ExternalConnection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Indica se la connessione può essere aggiornata in background (in modo asincrono). true se l'utilizzo preferito della connessione prevede l'aggiornamento asincrono in background; false se l'utilizzo preferito della connessione prevede l'aggiornamento sincrono in primo piano. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Specifica la descrizione utente per questa connessione |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Specifica l'identificatore univoco di questa connessione. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Specifica il metodo di autenticazione da utilizzare per stabilire (o ristabilire) la connessione. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Ottiene l'ID della connessione. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Indica se la connessione alla cartella di lavoro associata è stata eliminata. true se la connessione è stata eliminata; in caso contrario, falso. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | True se la connessione non è stata aggiornata per la prima volta; altrimenti falso. Questo stato può verificarsi quando l'utente salva il file prima che una query sia terminata. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Vero quando l'applicazione del foglio di calcolo dovrebbe tentare di mantenere aperta la connessione . Se false, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Specifica il percorso completo del file di connessione esterno da cui è stata creata questa connessione . Se una connessione non riesce durante un tentativo di aggiornamento dei dati e reconnectionMethod=1, , l'applicazione del foglio di calcolo tenterà di nuovo utilizzando le informazioni dal file di connessione esterno invece dell'oggetto di connessione incorporato nella cartella di lavoro. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Indica se l'applicazione del foglio di calcolo deve utilizzare sempre e solo le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione del foglio di calcolo dovrebbe seguire la procedura indicata dall'attributo reconnectionMethod |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Ottiene[`ConnectionParameterCollection`](../connectionparametercollection) per una query ODBC o Web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Ottiene la definizione della formula della query di alimentazione. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione non riesce. Il valore predefinito è ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | True se questa connessione deve essere aggiornata all'apertura del file; in caso contrario, falso. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti falso. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True se la password deve essere salvata come parte della stringa di connessione; in caso contrario, Falso. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Utilizzato quando l'origine dati esterna è basata su file. Quando una connessione a tale origine dati non riesce, l'applicazione del foglio di calcolo tenta di connettersi direttamente a questo file. Può essere espresso nell'URI o nella notazione del percorso del file specifica del sistema. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server spreadsheetML intermedio e l'origine dati esterna. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Ottiene o imposta il tipo DataSource della connessione esterna. |

### Guarda anche

* spazio dei nomi [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
