---
title: "Klass DBConnection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.DBConnection‑klass. Anger alla egenskaper som är associerade med en ODBC‑ eller OLE DB‑extern datakoppling"
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Anger alla egenskaper som är associerade med en extern ODBC- eller OLE DB-datakoppling.

```csharp
public class DBConnection : ExternalConnection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indikerar om anslutningen kan uppdateras i bakgrunden (asynkront). true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; false om föredragen användning är att uppdatera synkront i förgrunden. (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/dbconnection/classtype/) { get; } | Hämtar typen av detta [`ExternalConnection`](../externalconnection/)‑objekt. |
| override [Command](../../aspose.cells.externalconnections/dbconnection/command/) { get; set; } | Strängen som innehåller databaskommandot att skicka till data‑leverantörens API som kommer att interagera med den externa källan för att hämta data |
| override [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype/) { get; set; } | Anger OLE DB‑kommandotypen. 1. Frågan specificerar ett kubnamn 2. Frågan specificerar ett SQL‑uttryck 3. Frågan specificerar ett tabellnamn 4. Frågan specificerar att standardinformation har givits, och det är upp till leverantören hur den ska tolkas. 5. Frågan är mot en webbaserad List Data Provider. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Anger användarbeskrivningen för denna anslutning (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Hämtar anslutningsfilen. (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Anger det unika identifieraren för denna anslutning. (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo/) { get; set; } | (**Obsolete.**) Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla. |
| override [ConnectionString](../../aspose.cells.externalconnections/dbconnection/connectionstring/) { get; set; } | Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras). (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras). (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Hämtar anslutningens id. (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indikerar om den associerade arbetsboksanslutningen har raderats. true om anslutningen har raderats; annars false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True om anslutningen inte har uppdaterats för första gången; annars false. Detta tillstånd kan uppstå när användaren sparar filen innan en fråga har slutfört återlämnandet.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True när kalkylbladsapplikationen bör göra ansträngningar för att hålla anslutningen öppen. När false ska applikationen stänga anslutningen efter att informationen har hämtats.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Anger namnet på anslutningen. Varje anslutning måste ha ett unikt namn.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1, kommer kalkylbladsapplikationen att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indikerar om kalkylbladsapplikationen alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile-attributet när anslutningen uppdateras. Om false ska kalkylbladsapplikationen följa proceduren som anges av reconnectionMethod-attributet.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Hämtar [`ConnectionParameterCollection`](../connectionparametercollection/) för en ODBC- eller webbfråga.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula/) { get; } | Hämtar definitionen av power query-formeln. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Anger antalet minuter mellan automatiska uppdateringar av anslutningen.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True om denna anslutning ska uppdateras när filen öppnas; annars false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True om lösenordet ska sparas som en del av anslutningssträngen; annars False.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [SecondCommand](../../aspose.cells.externalconnections/dbconnection/secondcommand/) { get; set; } | Anger en andra kommandotextsträng som bevaras när PivotTable-serverbaserade sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE-klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor konstrueras |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand/) { get; set; } | (**Obsolete.**) Anger en andra kommandotextsträng som sparas när PivotTable‑serverbaserade sidfält används. För ODBC‑anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE‑klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor konstrueras. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylbladsprogrammet att ansluta direkt till den här filen. Kan uttryckas i URI‑ eller system‑specifik filsökvägsnotation. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Hämtar eller anger den externa anslutningens DataSource‑typ. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML‑server och den externa datakällan. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Hämtar eller anger den externa anslutningens DataSource‑typ. (Inherited from [`ExternalConnection`](../externalconnection/).) |

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en ny DBConnection‑instans genom att lägga till den i samlingen
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Ställ in grundläggande egenskaper
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Visa skrivskyddade egenskaper
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                Console.WriteLine("ConnectionString: " + dbConnection.ConnectionString);
                Console.WriteLine("CommandType: " + dbConnection.CommandType);
                Console.WriteLine("Command: " + dbConnection.Command);

                // Spara arbetsboken
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

### Se även

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


