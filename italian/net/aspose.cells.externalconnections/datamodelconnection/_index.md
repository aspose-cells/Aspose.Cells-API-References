---
title: "Classe DataModelConnection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ExternalConnections.DataModelConnection. Specifica una connessione al modello dati"
type: docs
url: /it/net/aspose.cells.externalconnections/datamodelconnection/
---
## DataModelConnection class

Specifica una connessione al modello di dati

```csharp
public class DataModelConnection : ExternalConnection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronicamente in background; false se l'uso preferito è aggiornare sincronicamente in primo piano. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/datamodelconnection/classtype/) { get; } | Restituisce il tipo di questo oggetto [`ExternalConnection`](../externalconnection/). |
| override [Command](../../aspose.cells.externalconnections/datamodelconnection/command/) { get; set; } | La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati |
| override [CommandType](../../aspose.cells.externalconnections/datamodelconnection/commandtype/) { get; set; } | Restituisce il tipo [`OLEDBCommandType`](../oledbcommandtype/). |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Specifica la descrizione utente per questa connessione (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Restituisce il file di connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsoleto.**) Specifica l'identificatore univoco di questa connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionString](../../aspose.cells.externalconnections/datamodelconnection/connectionstring/) { get; set; } | La stringa di informazioni della connessione è usata per contattare una fonte dati OLE DB o ODBC. |
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
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Ottiene la definizione della formula Power Query.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True se questa connessione deve essere aggiornata all'apertura del file; altrimenti, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True se la password deve essere salvata come parte della stringa di connessione; altrimenti, False.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Specifica una seconda stringa di testo del comando che viene conservata quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (non è presente alcuna clausola WHERE nella prima). Sulla base di questi 2 comandi (Command e ServerCommand), l'interfaccia utente dei parametri può essere popolata e le query parametrizzate possono essere costruite (Ereditato da [`ExternalConnection`](../externalconnection/).) |
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
    using System.Collections.Generic;

    public class ExternalConnectionsClassDataModelConnectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();

            try
            {
                // Crea un'istanza della classe DataModelConnection utilizzando la riflessione
                DataModelConnection connection = (DataModelConnection)System.Runtime.Serialization.FormatterServices.GetUninitializedObject(typeof(DataModelConnection));

                // Imposta le proprietà essenziali
                connection.Command = "SELECT * FROM Products";
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Aggiungi la connessione alle connessioni dati della cartella di lavoro
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Visualizza le informazioni sulla connessione
                Console.WriteLine($"Connection Type: {connection.ClassType}");
                Console.WriteLine($"Command: {connection.Command}");
                Console.WriteLine($"Command Type: {connection.CommandType}");
                Console.WriteLine($"Connection String: {connection.ConnectionString}");

                // Salva la cartella di lavoro
                workbook.Save("DataModelConnectionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with DataModelConnection.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DataModelConnection: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


