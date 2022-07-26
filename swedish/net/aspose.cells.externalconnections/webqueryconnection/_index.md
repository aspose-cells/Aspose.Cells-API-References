---
title: WebQueryConnection
second_title: Aspose.Cells för .NET API-referens
description: Anger egenskaperna för en webbfrågekälla. En webbfråga hämtar data från HTML-tabeller och kan även tillhandahålla HTTP Get-parametrar som ska bearbetas av webbservern för att generera HTML av inklusive parametrarna och parameterelementen.
type: docs
weight: 3350
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Anger egenskaperna för en webbfrågekälla. En webbfråga hämtar data från HTML-tabeller, och kan även tillhandahålla HTTP "Get"-parametrar som ska bearbetas av webbservern för att generera HTML av inklusive parametrarna och parameterelementen.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Indikerar om anslutningen kan uppdateras i bakgrunden (asynkront). true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Anger användarbeskrivningen för denna anslutning |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Anger den unika identifieraren för denna anslutning. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Anger den autentiseringsmetod som ska användas när anslutningen upprättas (eller återupprättas). |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage) { get; set; } | URL-adressen till den användarvända webbsidan som visar webbfrågans data. Denna URL är persisted om sourceData="true" och url har omdirigerats för att referera till en XML-fil. Sedan kan sidan som är vänd mot användaren visas i användargränssnittet och XML-data kan hämtas bakom kulisserna. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat) { get; set; } | Hur man hanterar formatering från HTML-källan när webbfrågedata överförs till kalkylbladet . Relevant när källdata är sant. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Hämtar id för anslutningen. |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive) { get; set; } | Flagga som anger om på varandra följande avgränsare ska behandlas som bara en avgränsare. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Indikerar om den associerade arbetsboksanslutningen har tagits bort. sant om anslutningen har tagits bort; annars, false. |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables) { get; set; } | Flagga som anger om webbfrågor endast ska fungera på HTML-tabeller. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | Sant om anslutningen inte har uppdaterats för första gången; annars falskt. Det här tillståndet kan inträffa när användaren sparar filen innan en fråga har slutat returnera. |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre) { get; set; } | Flagga som anger om data som finns i HTML PRE-taggar på webbsidan tolkas i kolumner när du importerar sidan till en frågetabell. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings) { get; set; } | Flagga som anger om alla tabeller i ett PRE-block ska analyseras med samma breddinställningar som den första raden. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates) { get; set; } | Flagga som anger om datum ska importeras till celler i kalkylbladet som text snarare än datum. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000) { get; set; } | Den här flaggan finns för bakåtkompatibilitet med äldre befintliga kalkylarksfiler och är satt till true om denna webbfråga uppdaterades i ett kalkylarksprogram som är nyare än eller lika med Microsoft Excel 2000. Detta är ett valfritt attribut som kan ignoreras_x00d_x00d. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97) { get; set; } | Den här flaggan finns för bakåtkompatibilitet med äldre befintliga kalkylbladsfiler och är satt till true om den här webbfrågan skapades i Microsoft Excel 97. Detta är ett valfritt attribut som kan ignoreras. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml) { get; set; } | true om webbfrågekällan är XML (mot HTML), annars false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata) { get; set; } | Flagga som anger att XML-källdata ska importeras istället för själva HTML-tabellen. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Sant när kalkylprogrammet ska anstränga sig för att hålla anslutningen öppen. När det är falskt bör applikationen stänga anslutningen efter att ha hämtat informationen . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Anger namnet på anslutningen. Varje anslutning måste ha ett unikt namn. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Anger den fullständiga sökvägen till den externa anslutningsfilen från vilken anslutningen skapades. Om en anslutning misslyckas under ett försök att uppdatera data och reconnectionMethod=1, kommer kalkylarksapplikationen att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Indikerar om kalkylbladsapplikationen alltid och endast ska använda -anslutningsinformationen i den externa anslutningsfilen som indikeras av odcFile-attributet när anslutningen uppdateras. Om falskt bör kalkylarksapplikationen följa proceduren som anges av reconnectionMethod-attributet |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Blir[`ConnectionParameterCollection`](../connectionparametercollection) för en ODBC- eller webbfråga. |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post) { get; set; } | Returnerar eller ställer in strängen som används med postmetoden för att mata in data till en webbserver för att returnera data från en webbfråga. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Hämtar definitionen av power-frågeformel. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Anger vad kalkylarksapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Anger antalet minuter mellan automatiska uppdateringar av anslutningen. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | Sant om den här anslutningen ska uppdateras när filen öppnas; annars, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Sant om den externa data som hämtas via anslutningen för att fylla en tabell ska sparas med arbetsboken; annars falskt. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True om lösenordet ska sparas som en del av anslutningssträngen; annars, False. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas, försöker kalkylarksprogrammet att ansluta direkt till den här filen. Kan vara uttryckt i URI eller systemspecifik filsökvägsnotation. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Identifierare för enkel inloggning (SSO) som används för autentisering mellan en mellanliggande kalkylarkML-server och den externa datakällan. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Hämtar eller ställer in den externa anslutningens DataSource-typ. |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url) { get; set; } | URL att använda för att uppdatera externa data. |

### Se även

* class [ExternalConnection](../externalconnection)
* namnutrymme [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
