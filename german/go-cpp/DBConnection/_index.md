---
title: "DBConnection Klasse"
linktitle: "DBConnection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DBConnection Klasse. Kapselt das Objekt, das die dbconnection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/dbconnection/
---

## DBConnection class

Gibt alle mit einer ODBC‑ oder OLE‑DB‑externen Datenverbindung verbundenen Eigenschaften an.

```go

type DBConnection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewDBConnection](./newdbconnection/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetClassType](./getclasstype/) | Liefert den Typ dieses ExternalConnection-Objekts. |
| [GetConnectionString](./getconnectionstring/) | Die Verbindungszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen. |
| [SetConnectionString](./setconnectionstring/) | Die Verbindungszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen. |
| [GetPowerQueryFormula](./getpowerqueryformula/) | Ruft die Definition der Power‑Query‑Formel ab. |
| [GetCommandType](./getcommandtype/) | Gibt den OLE DB-Befehlstyp an.1. Abfrage gibt einen Würfelnamen an2. Abfrage gibt eine SQL-Anweisung an3. Abfrage gibt einen Tabellennamen an4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden, und es liegt am Anbieter, wie diese zu interpretieren sind.5. Abfrage erfolgt gegen einen webbasierten List Data Provider. |
| [SetCommandType](./setcommandtype/) | Gibt den OLE DB-Befehlstyp an.1. Abfrage gibt einen Würfelnamen an2. Abfrage gibt eine SQL-Anweisung an3. Abfrage gibt einen Tabellennamen an4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden, und es liegt am Anbieter, wie diese zu interpretieren sind.5. Abfrage erfolgt gegen einen webbasierten List Data Provider. |
| [GetCommand](./getcommand/) | Der String, der den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird und mit der externen Quelle interagiert, um Daten abzurufen. |
| [SetCommand](./setcommand/) | Der String, der den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird und mit der externen Quelle interagiert, um Daten abzurufen. |
| [GetSecondCommand](./getsecondcommand/) | Gibt eine zweite Befehlszeichenfolge an, die beibehalten wird, wenn PivotTable-Server-basierte Seitenfelder verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfangreichere Abfrage als command (keine WHERE-Klausel ist im Ersteren vorhanden). Basierend auf diesen 2 Befehlen (Command und ServerCommand) kann die parameter UI gefüllt und parametrisierte Abfragen erstellt werden. |
| [SetSecondCommand](./setsecondcommand/) | Gibt eine zweite Befehlszeichenfolge an, die beibehalten wird, wenn PivotTable-Server-basierte Seitenfelder verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfangreichere Abfrage als command (keine WHERE-Klausel ist im Ersteren vorhanden). Basierend auf diesen 2 Befehlen (Command und ServerCommand) kann die parameter UI gefüllt und parametrisierte Abfragen erstellt werden. |
| [GetId](./getid/) | Liefert die ID der Verbindung. |
| [GetSourceType](./getsourcetype/) | Liefert oder setzt den DataSource-Typ der externen Verbindung. |
| [SetSourceType](./setsourcetype/) | Liefert oder setzt den DataSource-Typ der externen Verbindung. |
| [GetSSOId](./getssoid/) | Bezeichner für Single Sign On (SSO), der für die Authentifizierung zwischen einem intermediate‑spreadsheetML‑Server und der externen Datenquelle verwendet wird. |
| [SetSSOId](./setssoid/) | Bezeichner für Single Sign On (SSO), der für die Authentifizierung zwischen einem intermediate‑spreadsheetML‑Server und der externen Datenquelle verwendet wird. |
| [GetSavePassword](./getsavepassword/) | True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls False. |
| [SetSavePassword](./setsavepassword/) | True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls False. |
| [GetSaveData](./getsavedata/) | True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit der Arbeitsmappe gespeichert werden sollen; andernfalls false. |
| [SetSaveData](./setsavedata/) | True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit der Arbeitsmappe gespeichert werden sollen; andernfalls false. |
| [GetRefreshOnLoad](./getrefreshonload/) | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls false. |
| [SetRefreshOnLoad](./setrefreshonload/) | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls false. |
| [GetReconnectionMethodType](./getreconnectionmethodtype/) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required. |
| [SetReconnectionMethodType](./setreconnectionmethodtype/) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required. |
| [GetOnlyUseConnectionFile](./getonlyuseconnectionfile/) | Gibt an, ob die Tabellenkalkulationsanwendung stets ausschließlich die Verbindungsinformationen in der externen Verbindungsdatei, die durch das Attribut odcFile angegeben ist, verwenden soll, wenn die Verbindung aktualisiert wird. Wenn false, sollte die Tabellenkalkulationsanwendung dem durch das Attribut reconnectionMethod angegebenen Verfahren folgen. |
| [SetOnlyUseConnectionFile](./setonlyuseconnectionfile/) | Gibt an, ob die Tabellenkalkulationsanwendung stets ausschließlich die Verbindungsinformationen in der externen Verbindungsdatei, die durch das Attribut odcFile angegeben ist, verwenden soll, wenn die Verbindung aktualisiert wird. Wenn false, sollte die Tabellenkalkulationsanwendung dem durch das Attribut reconnectionMethod angegebenen Verfahren folgen. |
| [GetOdcFile](./getodcfile/) | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung während eines Versuchs, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1, versucht die Tabellenkalkulationsanwendung erneut, die Informationen aus der externen Verbindungsdatei zu verwenden, anstatt das im Arbeitsbuch eingebettete Verbindungsobjekt. |
| [SetOdcFile](./setodcfile/) | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung während eines Versuchs, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1, versucht die Tabellenkalkulationsanwendung erneut, die Informationen aus der externen Verbindungsdatei zu verwenden, anstatt das im Arbeitsbuch eingebettete Verbindungsobjekt. |
| [GetSourceFile](./getsourcefile/) | Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, direkt zu dieser Datei zu verbinden. Kann als URI oder in systemabhängiger Dateipfadnotation angegeben werden. |
| [SetSourceFile](./setsourcefile/) | Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, direkt zu dieser Datei zu verbinden. Kann als URI oder in systemabhängiger Dateipfadnotation angegeben werden. |
| [IsNew](./isnew/) | True, wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage abgeschlossen ist. |
| [SetIsNew](./setisnew/) | True, wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage abgeschlossen ist. |
| [GetName](./getname/) | Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben. |
| [SetName](./setname/) | Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben. |
| [GetKeepAlive](./getkeepalive/) | True, wenn die Tabellenkalkulationsanwendung bemüht sein soll, die Verbindung offen zu halten. Wenn false, sollte die Anwendung die Verbindung nach dem Abrufen der Informationen schließen. |
| [SetKeepAlive](./setkeepalive/) | True, wenn die Tabellenkalkulationsanwendung bemüht sein soll, die Verbindung offen zu halten. Wenn false, sollte die Anwendung die Verbindung nach dem Abrufen der Informationen schließen. |
| [GetRefreshInternal](./getrefreshinternal/) | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an. |
| [SetRefreshInternal](./setrefreshinternal/) | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an. |
| [GetConnectionDescription](./getconnectiondescription/) | Gibt die Benutzerbeschreibung für diese Verbindung an |
| [SetConnectionDescription](./setconnectiondescription/) | Gibt die Benutzerbeschreibung für diese Verbindung an |
| [IsDeleted](./isdeleted/) | Gibt an, ob die zugehörige Arbeitsbuchverbindung gelöscht wurde. true, wenn die Verbindung gelöscht wurde; andernfalls false. |
| [SetIsDeleted](./setisdeleted/) | Gibt an, ob die zugehörige Arbeitsbuchverbindung gelöscht wurde. true, wenn die Verbindung gelöscht wurde; andernfalls false. |
| [GetCredentialsMethodType](./getcredentialsmethodtype/) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll. |
| [SetCredentialsMethodType](./setcredentialsmethodtype/) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll. |
| [GetBackgroundRefresh](./getbackgroundrefresh/) | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Nutzung der Verbindung darin besteht, im Hintergrund asynchron zu aktualisieren; false, wenn die bevorzugte Nutzung darin besteht, im Vordergrund synchron zu aktualisieren. |
| [SetBackgroundRefresh](./setbackgroundrefresh/) | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Nutzung der Verbindung darin besteht, im Hintergrund asynchron zu aktualisieren; false, wenn die bevorzugte Nutzung darin besteht, im Vordergrund synchron zu aktualisieren. |
| [GetParameters](./getparameters/) | Ruft die ConnectionParameterCollection für eine ODBC- oder Webabfrage ab. |
| [GetConnectionFile](./getconnectionfile/) | Liefert die Verbindungsdatei. |
