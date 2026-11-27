---
title: "Klassen ExternalConnection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.ExternalConnection-klass. Anger en extern datakoppling"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Anger en extern datakoppling

```csharp
public abstract class ExternalConnection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Anger om anslutningen kan uppdateras i bakgrunden (asynkront). true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden. |
| abstract [ClassType](../../aspose.cells.externalconnections/externalconnection/classtype/) { get; } | Hämtar typen av detta `ExternalConnection`-objekt. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | Strängen som innehåller databaskommandot att skicka till data‑leverantörens API som kommer att interagera med den externa källan för att hämta data |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Anger OLE DB‑kommandotypen. 1. Frågan specificerar ett kubnamn 2. Frågan specificerar ett SQL‑uttryck 3. Frågan specificerar ett tabellnamn 4. Frågan specificerar att standardinformation har givits, och det är upp till leverantören hur den ska tolkas. 5. Frågan är mot en webbaserad List Data Provider. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Anger användarbeskrivningen för denna anslutning |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Hämtar anslutningsfilen. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Anger det unika identifieraren för denna anslutning. |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Anger autentiseringsmetoden som ska användas när anslutningen upprättas (eller återupprättas). |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Anger autentiseringsmetoden som ska användas när anslutningen upprättas (eller återupprättas). |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Hämtar id för anslutningen. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indikerar om den associerade arbetsboksanslutningen har raderats. true om anslutningen har raderats; annars false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True om anslutningen inte har uppdaterats för första gången; annars false. Detta tillstånd kan uppstå när användaren sparar filen innan en fråga har slutförts. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True när kalkylbladsapplikationen bör göra ansträngningar för att hålla anslutningen öppen. När false ska applikationen stänga anslutningen efter att informationen har hämtats. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Anger namnet på anslutningen. Varje anslutning måste ha ett unikt namn. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1, kommer kalkylbladsapplikationen att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indikerar om kalkylbladsapplikationen alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile‑attributet när anslutningen uppdateras. Om false ska kalkylbladsapplikationen följa proceduren som anges av reconnectionMethod‑attributet. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Hämtar [`ConnectionParameterCollection`](../connectionparametercollection/) för en ODBC‑ eller webbfråga. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Hämtar definitionen av power query-formeln. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Anger antalet minuter mellan automatiska uppdateringar av anslutningen. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True om denna anslutning ska uppdateras när filen öppnas; annars false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars false. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True om lösenordet ska sparas som en del av anslutningssträngen; annars False. |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Anger en andra kommandotextsträng som bevaras när PivotTable-serverbaserade sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE-klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor konstrueras |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylbladsapplikationen ansluta direkt till den här filen. Kan uttryckas i URI‑ eller systemspecifik filsökvägsnotation. |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Hämtar eller anger den externa anslutningens DataSource‑typ. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML‑server och den externa datakällan. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Hämtar eller anger den externa anslutningens DataSource‑typ. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


