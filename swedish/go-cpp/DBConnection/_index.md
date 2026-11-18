---
title: "DBConnection-klass"
linktitle: "DBConnection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DBConnection-klass. Inkapslar objektet som representerar dbconnection i Go."
type: docs
weight: 200
url: /sv/go-cpp/dbconnection/
---

## DBConnection class

Specificerar alla egenskaper som är associerade med en ODBC‑ eller OLE DB‑extern datakoppling.

```go

type DBConnection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewDBConnection](./newdbconnection/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetClassType](./getclasstype/) | Hämtar typen av detta ExternalConnection-objekt. |
| [GetConnectionString](./getconnectionstring/) | Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla. |
| [SetConnectionString](./setconnectionstring/) | Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla. |
| [GetPowerQueryFormula](./getpowerqueryformula/) | Hämtar definitionen av power query‑formeln. |
| [GetCommandType](./getcommandtype/) | Anger OLE DB‑kommandotypen. 1. Frågan specificerar ett kubnamn 2. Frågan specificerar ett SQL‑uttryck 3. Frågan specificerar ett tabellnamn 4. Frågan specificerar att standardinformation har givits, och det är upp till leverantören att tolka den. 5. Frågan är mot en webbaserad List Data Provider. |
| [SetCommandType](./setcommandtype/) | Anger OLE DB‑kommandotypen. 1. Frågan specificerar ett kubnamn 2. Frågan specificerar ett SQL‑uttryck 3. Frågan specificerar ett tabellnamn 4. Frågan specificerar att standardinformation har givits, och det är upp till leverantören att tolka den. 5. Frågan är mot en webbaserad List Data Provider. |
| [GetCommand](./getcommand/) | Strängen som innehåller databaskommandot att skicka till dataleverantörens API som kommer att interagera med den externa källan för att hämta data |
| [SetCommand](./setcommand/) | Strängen som innehåller databaskommandot att skicka till dataleverantörens API som kommer att interagera med den externa källan för att hämta data |
| [GetSecondCommand](./getsecondcommand/) | Specificerar en andra kommandotextsträng som sparas när PivotTable server-baserade sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE‑klausul finns i den förra). Baserat på dessa 2 kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor kan konstrueras |
| [SetSecondCommand](./setsecondcommand/) | Specificerar en andra kommandotextsträng som sparas när PivotTable server-baserade sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE‑klausul finns i den förra). Baserat på dessa 2 kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor kan konstrueras |
| [GetId](./getid/) | Hämtar anslutningens id. |
| [GetSourceType](./getsourcetype/) | Hämtar eller anger den externa anslutningens DataSource-typ |
| [SetSourceType](./setsourcetype/) | Hämtar eller anger den externa anslutningens DataSource-typ |
| [GetSSOId](./getssoid/) | Identifierare för Single Sign On (SSO) som används för autentisering mellan en intermediate‑spreadsheetML‑server och den externa datakällan. |
| [SetSSOId](./setssoid/) | Identifierare för Single Sign On (SSO) som används för autentisering mellan en intermediate‑spreadsheetML‑server och den externa datakällan. |
| [GetSavePassword](./getsavepassword/) | Sant om lösenordet ska sparas som en del av anslutningssträngen; annars Falskt. |
| [SetSavePassword](./setsavepassword/) | Sant om lösenordet ska sparas som en del av anslutningssträngen; annars Falskt. |
| [GetSaveData](./getsavedata/) | Sant om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars falskt. |
| [SetSaveData](./setsavedata/) | Sant om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars falskt. |
| [GetRefreshOnLoad](./getrefreshonload/) | Sant om den här anslutningen ska uppdateras när filen öppnas; annars falskt. |
| [SetRefreshOnLoad](./setrefreshonload/) | Sant om den här anslutningen ska uppdateras när filen öppnas; annars falskt. |
| [GetReconnectionMethodType](./getreconnectionmethodtype/) | Anger vad kalkylbladsprogrammet ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required. |
| [SetReconnectionMethodType](./setreconnectionmethodtype/) | Anger vad kalkylbladsprogrammet ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required. |
| [GetOnlyUseConnectionFile](./getonlyuseconnectionfile/) | Indikerar om kalkylbladsprogrammet alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile-attributet när anslutningen uppdateras. Om falskt ska kalkylbladsprogrammet följa proceduren som anges av reconnectionMethod-attributet. |
| [SetOnlyUseConnectionFile](./setonlyuseconnectionfile/) | Indikerar om kalkylbladsprogrammet alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile-attributet när anslutningen uppdateras. Om falskt ska kalkylbladsprogrammet följa proceduren som anges av reconnectionMethod-attributet. |
| [GetOdcFile](./getodcfile/) | Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1, kommer kalkylbladsprogrammet att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken. |
| [SetOdcFile](./setodcfile/) | Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1, kommer kalkylbladsprogrammet att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken. |
| [GetSourceFile](./getsourcefile/) | Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylbladsprogrammet ansluta direkt till den här filen. Kan uttryckas som en URI eller i systemspecifik filsökvägsnotation. |
| [SetSourceFile](./setsourcefile/) | Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylbladsprogrammet ansluta direkt till den här filen. Kan uttryckas som en URI eller i systemspecifik filsökvägsnotation. |
| [IsNew](./isnew/) | Sant om anslutningen inte har uppdaterats för första gången; annars falskt. Detta tillstånd kan inträffa när användaren sparar filen innan en fråga har slutförts. |
| [SetIsNew](./setisnew/) | Sant om anslutningen inte har uppdaterats för första gången; annars falskt. Detta tillstånd kan inträffa när användaren sparar filen innan en fråga har slutförts. |
| [GetName](./getname/) | Anger anslutningens namn. Varje anslutning måste ha ett unikt namn. |
| [SetName](./setname/) | Anger anslutningens namn. Varje anslutning måste ha ett unikt namn. |
| [GetKeepAlive](./getkeepalive/) | Sant när kalkylbladsprogrammet bör göra ansträngningar för att hålla anslutningen öppen. När falskt ska programmet stänga anslutningen efter att informationen har hämtats. |
| [SetKeepAlive](./setkeepalive/) | Sant när kalkylbladsprogrammet bör göra ansträngningar för att hålla anslutningen öppen. När falskt ska programmet stänga anslutningen efter att informationen har hämtats. |
| [GetRefreshInternal](./getrefreshinternal/) | Anger antalet minuter mellan automatiska uppdateringar av anslutningen. |
| [SetRefreshInternal](./setrefreshinternal/) | Anger antalet minuter mellan automatiska uppdateringar av anslutningen. |
| [GetConnectionDescription](./getconnectiondescription/) | Anger användarens beskrivning för denna anslutning |
| [SetConnectionDescription](./setconnectiondescription/) | Anger användarens beskrivning för denna anslutning |
| [IsDeleted](./isdeleted/) | Indikerar om den associerade arbetsboksanslutningen har raderats. Sant om anslutningen har raderats; annars falskt. |
| [SetIsDeleted](./setisdeleted/) | Indikerar om den associerade arbetsboksanslutningen har raderats. Sant om anslutningen har raderats; annars falskt. |
| [GetCredentialsMethodType](./getcredentialsmethodtype/) | Anger autentiseringsmetoden som ska användas när anslutningen upprättas (eller återupprättas). |
| [SetCredentialsMethodType](./setcredentialsmethodtype/) | Anger autentiseringsmetoden som ska användas när anslutningen upprättas (eller återupprättas). |
| [GetBackgroundRefresh](./getbackgroundrefresh/) | Indikerar om anslutningen kan uppdateras i bakgrunden (asynkront). Sant om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; falskt om föredragen användning är att uppdatera synkront i förgrunden. |
| [SetBackgroundRefresh](./setbackgroundrefresh/) | Indikerar om anslutningen kan uppdateras i bakgrunden (asynkront). Sant om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; falskt om föredragen användning är att uppdatera synkront i förgrunden. |
| [GetParameters](./getparameters/) | Hämtar ConnectionParameterCollection för en ODBC‑ eller webbfråga. |
| [GetConnectionFile](./getconnectionfile/) | Hämtar anslutningsfilen. |
