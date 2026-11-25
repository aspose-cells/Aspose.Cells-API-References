---
title: "Classe WebQueryConnection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ExternalConnections.WebQueryConnection class. Specifica le proprietà per una sorgente di query web. Una query web recupererà dati dalle tabelle HTML e può anche fornire parametri HTTP Get da elaborare dal server web nella generazione dell'HTML includendo i parametri e gli elementi dei parametri"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Specifica le proprietà per una sorgente di query web. Una query web recupererà dati da tabelle HTML e può anche fornire parametri HTTP \"Get\" da elaborare dal server web nella generazione dell'HTML includendo i parametri e gli elementi dei parametri.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronicamente in background; false se l'uso preferito è aggiornare sincronicamente in primo piano. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/webqueryconnection/classtype/) { get; } | Restituisce il tipo di questo oggetto [`ExternalConnection`](../externalconnection/). |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la sorgente esterna per recuperare i dati (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Specifica il tipo di comando OLE DB. 1. La query specifica un nome del cubo 2. La query specifica un'istruzione SQL 3. La query specifica un nome della tabella 4. La query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. La query è contro un List Data Provider basato sul web. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Specifica la descrizione utente per questa connessione (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionFile](../../aspose.cells.externalconnections/webqueryconnection/connectionfile/) { get; } | Ottiene il file di connessione. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsoleto.**) Specifica l'identificatore univoco di questa connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | La stringa di informazioni di connessione è usata per stabilire un contatto con una fonte dati OLE DB o ODBC. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsoleto.**) Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o ristabilisce) la connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o ristabilisce) la connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage/) { get; set; } | (**Obsolete.**) L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL è conservato nel caso in cui sourceData=\"true\" e l'url sia stato reindirizzato per fare riferimento a un file XML. Allora la pagina destinata all'utente può essere mostrata nell'interfaccia, e i dati XML possono essere recuperati in background. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage/) { get; set; } | L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL è conservato nel caso in cui sourceData=\"true\" e l'url sia stato reindirizzato per fare riferimento a un file XML. Allora la pagina destinata all'utente può essere mostrata nell'interfaccia, e i dati XML possono essere recuperati in background. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat/) { get; set; } | Come gestire la formattazione dalla sorgente HTML quando si importano i dati della query web nel foglio di lavoro. Rilevante quando sourceData è True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Restituisce l'ID della connessione. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive/) { get; set; } | Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indica se la connessione della cartella di lavoro associata è stata eliminata. true se la connessione è stata eliminata; altrimenti, false. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables/) { get; set; } | Flag che indica se le query web devono funzionare solo su tabelle HTML. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True se la connessione non è stata aggiornata per la prima volta; altrimenti, false. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno dei dati. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre/) { get; set; } | Flag che indica se i dati contenuti nei tag HTML PRE nella pagina web vengono analizzati in colonne quando si importa la pagina in una tabella di query. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings/) { get; set; } | Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates/) { get; set; } | Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000/) { get; set; } | Questo flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostato su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. Questo è un attributo opzionale che può essere ignorato. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97/) { get; set; } | Questo flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostato su true se questa query web è stata creata in Microsoft Excel 97. Questo è un attributo opzionale che può essere ignorato. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml/) { get; set; } | true se la sorgente della query web è XML (invece di HTML), altrimenti false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/) { get; set; } | Flag che indica che i dati sorgente XML devono essere importati invece della tabella HTML stessa. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True quando l'applicazione di foglio di calcolo dovrebbe cercare di mantenere la connessione aperta. Quando false, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Specifica il nome della connessione. Ogni connessione deve avere un nome univoco. (Ereditato da [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Specifica il percorso completo al file di connessione esterno da cui è stata creata questa connessione. Se una connessione fallisce durante un tentativo di aggiornamento dei dati, e reconnectionMethod=1, l'applicazione di foglio di calcolo proverà di nuovo usando le informazioni dal file di connessione esterno invece dell'oggetto di connessione incorporato nella cartella di lavoro.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indica se l'applicazione di foglio di calcolo dovrebbe sempre e solo utilizzare le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione è aggiornata. Se false, l'applicazione di foglio di calcolo dovrebbe seguire la procedura indicata dall'attributo reconnectionMethod(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Ottiene [`ConnectionParameterCollection`](../connectionparametercollection/) per una query ODBC o web.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post/) { get; set; } | Restituisce o imposta la stringa usata con il metodo POST per inviare dati a un server web per restituire dati da una query web. |
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
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url/) { get; set; } | URL da utilizzare per aggiornare dati esterni. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassWebQueryConnectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Crea una connessione di query web tramite la collezione
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];
                
                connection.Url = "https://example.com/financial-data";
                connection.IsHtmlTables = true;
                connection.IsTextDates = true;
                connection.HtmlFormat = HtmlFormatHandlingType.All;

                Console.WriteLine($"Web query URL: {connection.Url}");
                Console.WriteLine($"HTML tables only: {connection.IsHtmlTables}");

                workbook.Save("WebQueryConnectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebQueryConnection: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


