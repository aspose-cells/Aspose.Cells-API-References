---
title: DBConnection
second_title: Aspose.Cells för .NET API-referens
description: Anger alla egenskaper som är associerade med en extern ODBC- eller OLE DB-dataanslutning.
type: docs
weight: 3280
url: /sv/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Anger alla egenskaper som är associerade med en extern ODBC- eller OLE DB-dataanslutning.

```csharp
public class DBConnection : ExternalConnection
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Indikerar om anslutningen kan uppdateras i bakgrunden (asynkront). true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden. |
| [Command](../../aspose.cells.externalconnections/dbconnection/command) { get; set; } | Strängen som innehåller databaskommandot som ska skickas till dataleverantörens API som kommer att interagera med den externa källan för att hämta data |
| [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype) { get; set; } | Anger OLE DB-kommandotypen. 1. Fråga anger ett kubnamn 2. Fråga anger en SQL-sats 3. Fråga anger ett tabellnamn 4. Fråga anger att standardinformation har getts, och det är upp till leverantören hur man tolkar._x00d. en webbaserad listdataleverantör. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Anger användarbeskrivningen för denna anslutning |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Anger den unika identifieraren för denna anslutning. |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo) { get; set; } | Anslutningsinformationssträngen används för att ta kontakt med en OLE DB- eller ODBC-datakälla. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Anger den autentiseringsmetod som ska användas när anslutningen upprättas (eller återupprättas). |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Hämtar id för anslutningen. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Indikerar om den associerade arbetsboksanslutningen har tagits bort. sant om anslutningen har tagits bort; annars, false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | Sant om anslutningen inte har uppdaterats för första gången; annars falskt. Det här tillståndet kan inträffa när användaren sparar filen innan en fråga har slutat returnera. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Sant när kalkylprogrammet ska anstränga sig för att hålla anslutningen öppen. När det är falskt bör applikationen stänga anslutningen efter att ha hämtat informationen . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Anger namnet på anslutningen. Varje anslutning måste ha ett unikt namn. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Anger den fullständiga sökvägen till den externa anslutningsfilen från vilken anslutningen skapades. Om en anslutning misslyckas under ett försök att uppdatera data och reconnectionMethod=1, kommer kalkylarksapplikationen att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Indikerar om kalkylbladsapplikationen alltid och endast ska använda -anslutningsinformationen i den externa anslutningsfilen som indikeras av odcFile-attributet när anslutningen uppdateras. Om falskt bör kalkylarksapplikationen följa proceduren som anges av reconnectionMethod-attributet |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Blir[`ConnectionParameterCollection`](../connectionparametercollection) för en ODBC- eller webbfråga. |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula) { get; } | Hämtar definitionen av power-frågeformel. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Anger vad kalkylarksapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Anger antalet minuter mellan automatiska uppdateringar av anslutningen. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | Sant om den här anslutningen ska uppdateras när filen öppnas; annars, false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Sant om den externa data som hämtas via anslutningen för att fylla en tabell ska sparas med arbetsboken; annars falskt. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True om lösenordet ska sparas som en del av anslutningssträngen; annars, False. |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand) { get; set; } | Anger en andra kommandotextsträng som kvarstår när PivotTable-serverbaserade sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än kommando (ingen WHERE-sats finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand), kan parameter UI fyllas i och parameteriserade frågor kan konstrueras |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas, försöker kalkylarksprogrammet att ansluta direkt till den här filen. Kan vara uttryckt i URI eller systemspecifik filsökvägsnotation. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Identifierare för enkel inloggning (SSO) som används för autentisering mellan en mellanliggande kalkylarkML-server och den externa datakällan. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Hämtar eller ställer in den externa anslutningens DataSource-typ. |

### Se även

* class [ExternalConnection](../externalconnection)
* namnutrymme [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
