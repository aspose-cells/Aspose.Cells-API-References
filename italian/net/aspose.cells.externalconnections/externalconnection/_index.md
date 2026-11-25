---
title: "Classe ExternalConnection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ExternalConnections.ExternalConnection class. Specifica una connessione dati esterna"
type: docs
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
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronamente in background; false se l'uso preferito della connessione è aggiornare sincronicamente in primo piano. |
| abstract [ClassType](../../aspose.cells.externalconnections/externalconnection/classtype/) { get; } | Ottiene il tipo di questo oggetto `ExternalConnection`. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Specifica il tipo di comando OLE DB. 1. La query specifica un nome di cubo 2. La query specifica un'istruzione SQL 3. La query specifica un nome di tabella 4. La query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. La query è rivolta a un provider di dati elenco basato sul web. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Specifica la descrizione utente per questa connessione |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Ottiene il file di connessione. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Specifica l'identificatore univoco di questa connessione. |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | La stringa di informazioni della connessione è usata per contattare una fonte dati OLE DB o ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Ottiene l'ID della connessione. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indica se la connessione del workbook associata è stata eliminata. true se la connessione è stata eliminata; altrimenti, false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True se la connessione non è stata ancora aggiornata per la prima volta; altrimenti, false. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno dei dati. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True quando l'applicazione di foglio di calcolo dovrebbe impegnarsi a mantenere la connessione aperta. Quando false, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Specifica il percorso completo al file di connessione esterna da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati, e reconnectionMethod=1, allora l'applicazione di foglio di calcolo proverà di nuovo usando le informazioni dal file di connessione esterna invece dell'oggetto connessione incorporato nel workbook. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indica se l'applicazione di foglio di calcolo dovrebbe sempre e solo utilizzare le informazioni di connessione nel file di connessione esterna indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione di foglio di calcolo dovrebbe seguire la procedura indicata dall'attributo reconnectionMethod. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Ottiene [`ConnectionParameterCollection`](../connectionparametercollection/) per una query ODBC o web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Ottiene la definizione della formula Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Specifica il numero di minuti tra gli aggiornamenti automatici della connessione. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True se questa connessione deve essere aggiornata all'apertura del file; altrimenti, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True se i dati esterni recuperati tramite la connessione per popolare una tabella devono essere salvati con la cartella di lavoro; altrimenti, false. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True se la password deve essere salvata come parte della stringa di connessione; altrimenti, False. |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Utilizzato quando la fonte di dati esterna è basata su file. Quando una connessione a tale fonte di dati fallisce, l'applicazione di foglio di calcolo tenta di connettersi direttamente a questo file. Può essere espresso in formato URI o notazione di percorso file specifica del sistema. |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Ottiene o imposta il tipo di DataSource della connessione esterna. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identificatore per Single Sign On (SSO) utilizzato per l'autenticazione tra un server spreadsheetML intermedio e la fonte di dati esterna. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Ottiene o imposta il tipo di DataSource della connessione esterna. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionDemo
    {
        public static void Run()
        {
            string sourceDir = "Your Source Directory";

            Workbook workbook = new Workbook(sourceDir + "example.xlsx");
            ExternalConnectionCollection conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }

            workbook = new Workbook(sourceDir + "example.xlsm");
            conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


