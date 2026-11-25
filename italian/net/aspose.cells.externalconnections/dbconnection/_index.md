---
title: "Classe DBConnection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe **Aspose.Cells.ExternalConnections.DBConnection**. Specifica tutte le proprietà associate a una connessione dati esterna ODBC o OLE DB"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Specifica tutte le proprietà associate a una connessione dati esterna ODBC o OLE DB.

```csharp
public class DBConnection : ExternalConnection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronicamente in background; false se l'uso preferito è aggiornare sincronicamente in primo piano. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/dbconnection/classtype/) { get; } | Restituisce il tipo di questo oggetto [`ExternalConnection`](../externalconnection/). |
| override [Command](../../aspose.cells.externalconnections/dbconnection/command/) { get; set; } | La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati |
| override [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype/) { get; set; } | Specifica il tipo di comando OLE DB. 1. La query specifica un nome di cubo 2. La query specifica un'istruzione SQL 3. La query specifica un nome di tabella 4. La query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. La query è rivolta a un provider di dati elenco basato sul web. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Specifica la descrizione utente per questa connessione (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Restituisce il file di connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsoleto.**) Specifica l'identificatore univoco di questa connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo/) { get; set; } | (**Obsoleto.**) La stringa di informazioni della connessione è usata per contattare una fonte dati OLE DB o ODBC. |
| override [ConnectionString](../../aspose.cells.externalconnections/dbconnection/connectionstring/) { get; set; } | La stringa di informazioni della connessione è usata per contattare una fonte dati OLE DB o ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsoleto.**) Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o ristabilisce) la connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o ristabilisce) la connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Restituisce l'ID della connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indica se la connessione della cartella di lavoro associata è stata eliminata. true se la connessione è stata eliminata; altrimenti, false. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True se la connessione non è stata aggiornata per la prima volta; altrimenti, false. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno dei dati. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True quando l'applicazione di foglio di calcolo dovrebbe cercare di mantenere la connessione aperta. Quando false, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Specifica il percorso completo al file di connessione esterno da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati, e reconnectionMethod=1, l'applicazione di foglio di calcolo proverà di nuovo usando le informazioni dal file di connessione esterno invece dell'oggetto di connessione incorporato nella cartella di lavoro.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indica se l'applicazione di foglio di calcolo dovrebbe sempre e solo utilizzare le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione è aggiornata. Se false, l'applicazione di foglio di calcolo dovrebbe seguire la procedura indicata dall'attributo reconnectionMethod(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Ottiene [`ConnectionParameterCollection`](../connectionparametercollection/) per una query ODBC o web.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula/) { get; } | Ottiene la definizione della formula Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True se questa connessione deve essere aggiornata all'apertura del file; altrimenti, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True se la password deve essere salvata come parte della stringa di connessione; altrimenti, False.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [SecondCommand](../../aspose.cells.externalconnections/dbconnection/secondcommand/) { get; set; } | Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand/) { get; set; } | (**Obsolete.**) Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Utilizzato quando la fonte dati esterna è basata su file. Quando una connessione a tale fonte dati fallisce, l'applicazione di foglio di calcolo tenta di connettersi direttamente a questo file. May be expressed in URI or system-specific file path notation.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Ottiene o imposta il tipo di DataSource della connessione esterna.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server intermedio spreadsheetML e la fonte dati esterna.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Ottiene o imposta il tipo di DataSource della connessione esterna.(Inherited from [`ExternalConnection`](../externalconnection/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassDBConnectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una nuova istanza DBConnection aggiungendola alla collezione
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Imposta le proprietà di base
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Visualizza le proprietà in sola lettura
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                Console.WriteLine("ConnectionString: " + dbConnection.ConnectionString);
                Console.WriteLine("CommandType: " + dbConnection.CommandType);
                Console.WriteLine("Command: " + dbConnection.Command);

                // Salva la cartella di lavoro
                workbook.Save("DBConnectionDemo.xlsx");
                Console.WriteLine("DBConnection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DBConnection: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


