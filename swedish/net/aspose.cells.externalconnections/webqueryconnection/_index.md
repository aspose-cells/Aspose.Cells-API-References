---
title: "Klass WebQueryConnection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.WebQueryConnection‑klass. Anger egenskaperna för en webbfrågekälla. En webbfråga hämtar data från HTML‑tabeller och kan även leverera HTTP‑Get‑parametrar som ska bearbetas av webbservern vid generering av HTML genom att inkludera parametrarna och parameterelementen."
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Anger egenskaperna för en webbfrågekälla. En webbfråga hämtar data från HTML-tabeller och kan även leverera HTTP \"Get\"-parametrar som behandlas av webbservern vid generering av HTML genom att inkludera parametrarna och parameterelementen.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indikerar om anslutningen kan uppdateras i bakgrunden (asynkront). true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; false om föredragen användning är att uppdatera synkront i förgrunden. (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/webqueryconnection/classtype/) { get; } | Hämtar typen av detta [`ExternalConnection`](../externalconnection/)‑objekt. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | Strängen som innehåller databaskommandot att skicka till data‑leverantörens API som kommer att interagera med den externa källan för att hämta data (ärvd från [`ExternalConnection`](../externalconnection/).) |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Anger OLE DB‑kommandotypen. 1. Fråga anger ett kubnamn 2. Fråga anger ett SQL‑uttryck 3. Fråga anger ett tabellnamn 4. Fråga anger att standardinformation har givits, och det är upp till leverantören hur den ska tolkas. 5. Fråga är mot en webb‑baserad List Data Provider. (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Anger användarbeskrivningen för denna anslutning (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionFile](../../aspose.cells.externalconnections/webqueryconnection/connectionfile/) { get; } | Hämtar anslutningsfilen. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Anger det unika identifieraren för denna anslutning. (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | Anslutningsinformationssträngen används för att kontakta en OLE DB- eller ODBC-datakälla.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras). (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Anger autentiseringsmetoden som ska användas när anslutningen etableras (eller återetableras). (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage/) { get; set; } | (**Obsolete.**) URL:en för den användarorienterade webbsidan som visar webbfrågedata. Denna URL sparas om sourceData=\"true\" och url har omdirigerats för att referera till en XML-fil. Då kan den användarorienterade sidan visas i UI:t, och XML-data kan hämtas i bakgrunden. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage/) { get; set; } | URL:en för den användarorienterade webbsidan som visar webbfrågedata. Denna URL sparas om sourceData=\"true\" och url har omdirigerats för att referera till en XML-fil. Då kan den användarorienterade sidan visas i UI:t, och XML-data kan hämtas i bakgrunden. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat/) { get; set; } | Hur formatering från HTML-källan ska hanteras när webbfrågedata förs in i kalkylbladet. Relevant när sourceData är True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Hämtar anslutningens id. (Ärvd från [`ExternalConnection`](../externalconnection/).) |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive/) { get; set; } | Flagga som anger om på varandra följande avgränsare ska behandlas som en enda avgränsare. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indikerar om den associerade arbetsboksanslutningen har raderats. true om anslutningen har raderats; annars false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables/) { get; set; } | Flagga som anger om webbfrågor endast ska fungera på HTML-tabeller. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True om anslutningen inte har uppdaterats för första gången; annars false. Detta tillstånd kan uppstå när användaren sparar filen innan en fråga har slutfört återlämnandet.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre/) { get; set; } | Flagga som anger om data som finns inom HTML PRE-taggar på webbsidan ska parsas till kolumner när du importerar sidan till en frågetabell. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings/) { get; set; } | Flagga som anger om alla tabeller inom ett PRE-block ska parsas med samma breddinställningar som den första raden. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates/) { get; set; } | Flagga som anger om datum ska importeras till celler i kalkylbladet som text istället för som datum. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000/) { get; set; } | Denna flagga finns för bakåtkompatibilitet med äldre befintliga kalkylbladsfiler, och sätts till true om denna webbfråga uppdaterades i ett kalkylbladsprogram nyare än eller lika med Microsoft Excel 2000. Detta är ett valfritt attribut som kan ignoreras. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97/) { get; set; } | Denna flagga finns för bakåtkompatibilitet med äldre befintliga kalkylbladsfiler, och sätts till true om denna webbfråga skapades i Microsoft Excel 97. Detta är ett valfritt attribut som kan ignoreras. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml/) { get; set; } | true om webbfrågekällan är XML (i stället för HTML), annars false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/) { get; set; } | Flagga som anger att XML-källdata ska importeras i stället för själva HTML-tabellen. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True när kalkylbladsapplikationen bör göra ansträngningar för att hålla anslutningen öppen. När false ska applikationen stänga anslutningen efter att informationen har hämtats.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Anger namnet på anslutningen. Varje anslutning måste ha ett unikt namn.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1, kommer kalkylbladsapplikationen att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indikerar om kalkylbladsapplikationen alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile-attributet när anslutningen uppdateras. Om false ska kalkylbladsapplikationen följa proceduren som anges av reconnectionMethod-attributet.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Hämtar [`ConnectionParameterCollection`](../connectionparametercollection/) för en ODBC- eller webbfråga.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post/) { get; set; } | Returnerar eller anger strängen som används med POST-metoden för att skicka data till en webbserver för att returnera data från en webbfråga. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Hämtar definitionen av power‑query‑formeln. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Anger antalet minuter mellan automatiska uppdateringar av anslutningen.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True om denna anslutning ska uppdateras när filen öppnas; annars false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True om lösenordet ska sparas som en del av anslutningssträngen; annars False.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Anger en andra kommandotextsträng som sparas när PivotTable‑serverbaserade sidfält används. För ODBC‑anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE‑klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor konstrueras (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylbladsprogrammet att ansluta direkt till den här filen. Kan uttryckas i URI‑ eller system‑specifik filsökvägsnotation. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Hämtar eller anger den externa anslutningens DataSource‑typ. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identifierare för Single Sign On (SSO) som används för autentisering mellan en mellanliggande spreadsheetML‑server och den externa datakällan. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Hämtar eller anger den externa anslutningens DataSource‑typ. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url/) { get; set; } | URL att använda för att uppdatera extern data. |

### Exempel

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
                // Skapa webbfrågeanslutning via samling
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

### Se även

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


