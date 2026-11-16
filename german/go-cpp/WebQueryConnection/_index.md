---
title: "WebQueryConnection Klasse"
linktitle: "WebQueryConnection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "WebQueryConnection Klasse. Kapselt das Objekt, das webqueryconnection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/webqueryconnection/
---

## WebQueryConnection class

Gibt die Eigenschaften für eine Webabfrage‑Quelle an. Eine Webabfrage ruft Daten aus HTML‑Tabellen ab und kann außerdem HTTP "Get"-Parameter bereitstellen, die vom Webserver bei der Generierung des HTML unter Einbeziehung der Parameter und Parameter‑Elemente verarbeitet werden.

```go

type WebQueryConnection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewWebQueryConnection](./newwebqueryconnection/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetClassType](./getclasstype/) | Liefert den Typ dieses ExternalConnection-Objekts. |
| [IsXml](./isxml/) | true, wenn die Webabfragequelle XML (statt HTML) ist, andernfalls false. |
| [SetIsXml](./setisxml/) | true, wenn die Webabfragequelle XML (statt HTML) ist, andernfalls false. |
| [IsXl97](./isxl97/) | Dieses Flag existiert aus Gründen der Abwärtskompatibilität mit älteren bestehenden Tabellenkalkulationsdateien und ist auf true gesetzt, wenn diese Webabfrage in Microsoft Excel 97 erstellt wurde. Dies ist ein optionales Attribut, das ignoriert werden kann. |
| [SetIsXl97](./setisxl97/) | Dieses Flag existiert aus Gründen der Abwärtskompatibilität mit älteren bestehenden Tabellenkalkulationsdateien und ist auf true gesetzt, wenn diese Webabfrage in Microsoft Excel 97 erstellt wurde. Dies ist ein optionales Attribut, das ignoriert werden kann. |
| [IsXl2000](./isxl2000/) | Dieses Flag existiert aus Gründen der Abwärtskompatibilität mit älteren bestehenden Tabellenkalkulationsdateien und ist auf true gesetzt, wenn diese Webabfrage in einer Tabellenkalkulationsanwendung, die neuer oder gleich Microsoft Excel 2000 ist, aktualisiert wurde. Dies ist ein optionales Attribut, das ignoriert werden kann. |
| [SetIsXl2000](./setisxl2000/) | Dieses Flag existiert aus Gründen der Abwärtskompatibilität mit älteren bestehenden Tabellenkalkulationsdateien und ist auf true gesetzt, wenn diese Webabfrage in einer Tabellenkalkulationsanwendung, die neuer oder gleich Microsoft Excel 2000 ist, aktualisiert wurde. Dies ist ein optionales Attribut, das ignoriert werden kann. |
| [GetUrl](./geturl/) | URL, die zum Aktualisieren externer Daten verwendet wird. |
| [SetUrl](./seturl/) | URL, die zum Aktualisieren externer Daten verwendet wird. |
| [GetConnectionFile](./getconnectionfile/) | Liefert die Verbindungsdatei. |
| [IsTextDates](./istextdates/) | Flag, das angibt, ob Datumswerte als Text statt als Datum in Zellen des Arbeitsblatts importiert werden sollen. |
| [SetIsTextDates](./setistextdates/) | Flag, das angibt, ob Datumswerte als Text statt als Datum in Zellen des Arbeitsblatts importiert werden sollen. |
| [IsXmlSourceData](./isxmlsourcedata/) | Flag, das angibt, dass XML-Quelldaten anstelle der HTML-Tabelle selbst importiert werden sollen. |
| [SetIsXmlSourceData](./setisxmlsourcedata/) | Flag, das angibt, dass XML-Quelldaten anstelle der HTML-Tabelle selbst importiert werden sollen. |
| [GetPost](./getpost/) | Gibt die Zeichenkette zurück oder setzt sie, die mit der POST-Methode zum Eingeben von Daten in einen Webserver verwendet wird, um Daten aus einer Webabfrage zurückzugeben. |
| [SetPost](./setpost/) | Gibt die Zeichenkette zurück oder setzt sie, die mit der POST-Methode zum Eingeben von Daten in einen Webserver verwendet wird, um Daten aus einer Webabfrage zurückzugeben. |
| [IsParsePre](./isparsepre/) | Flag, das angibt, ob Daten, die innerhalb von HTML-PRE-Tags auf der Webseite enthalten sind, beim Importieren der Seite in eine Abfragetabelle in Spalten aufgeteilt werden. |
| [SetIsParsePre](./setisparsepre/) | Flag, das angibt, ob Daten, die innerhalb von HTML-PRE-Tags auf der Webseite enthalten sind, beim Importieren der Seite in eine Abfragetabelle in Spalten aufgeteilt werden. |
| [IsHtmlTables](./ishtmltables/) | Flag, das angibt, ob Webabfragen nur mit HTML-Tabellen funktionieren sollen. |
| [SetIsHtmlTables](./setishtmltables/) | Flag, das angibt, ob Webabfragen nur mit HTML-Tabellen funktionieren sollen. |
| [GetHtmlFormat](./gethtmlformat/) | Wie die Formatierung aus der HTML-Quelle beim Einbringen von Webabfragedaten in das Arbeitsblatt behandelt wird. Relevant, wenn sourceData True ist. |
| [SetHtmlFormat](./sethtmlformat/) | Wie die Formatierung aus der HTML-Quelle beim Einbringen von Webabfragedaten in das Arbeitsblatt behandelt wird. Relevant, wenn sourceData True ist. |
| [IsSameSettings](./issamesettings/) | Flag, das angibt, ob alle Tabellen innerhalb eines PRE-Blocks mit denselben Breiteneinstellungen wie die erste Zeile geparst werden sollen. |
| [SetIsSameSettings](./setissamesettings/) | Flag, das angibt, ob alle Tabellen innerhalb eines PRE-Blocks mit denselben Breiteneinstellungen wie die erste Zeile geparst werden sollen. |
| [GetEditWebPage](./geteditwebpage/) | Die URL der benutzerorientierten Webseite, die die Webabfragedaten anzeigt. Diese URL wird gespeichert, falls sourceData=\"true\" ist und die URL zu einer XML-Datei umgeleitet wurde. Dann kann die benutzerorientierte Seite in der UI angezeigt werden, und die XML-Daten können im Hintergrund abgerufen werden. |
| [SetEditWebPage](./seteditwebpage/) | Die URL der benutzerorientierten Webseite, die die Webabfragedaten anzeigt. Diese URL wird gespeichert, falls sourceData=\"true\" ist und die URL zu einer XML-Datei umgeleitet wurde. Dann kann die benutzerorientierte Seite in der UI angezeigt werden, und die XML-Daten können im Hintergrund abgerufen werden. |
| [IsConsecutive](./isconsecutive/) | Flag, das angibt, ob aufeinanderfolgende Trennzeichen als ein einziges Trennzeichen behandelt werden sollen. |
| [SetIsConsecutive](./setisconsecutive/) | Flag, das angibt, ob aufeinanderfolgende Trennzeichen als ein einziges Trennzeichen behandelt werden sollen. |
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
| [GetPowerQueryFormula](./getpowerqueryformula/) | Ruft die Definition der Power‑Query‑Formel ab. |
| [GetCommand](./getcommand/) | Der String, der den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird und mit der externen Quelle interagiert, um Daten abzurufen. |
| [SetCommand](./setcommand/) | Der String, der den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird und mit der externen Quelle interagiert, um Daten abzurufen. |
| [GetCommandType](./getcommandtype/) | Gibt den OLE DB-Befehlstyp an.1. Abfrage gibt einen Würfelnamen an2. Abfrage gibt eine SQL-Anweisung an3. Abfrage gibt einen Tabellennamen an4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden, und es liegt am Anbieter, wie diese zu interpretieren sind.5. Abfrage erfolgt gegen einen webbasierten List Data Provider. |
| [SetCommandType](./setcommandtype/) | Gibt den OLE DB-Befehlstyp an.1. Abfrage gibt einen Würfelnamen an2. Abfrage gibt eine SQL-Anweisung an3. Abfrage gibt einen Tabellennamen an4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden, und es liegt am Anbieter, wie diese zu interpretieren sind.5. Abfrage erfolgt gegen einen webbasierten List Data Provider. |
| [GetConnectionString](./getconnectionstring/) | Die Verbindungszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen. |
| [SetConnectionString](./setconnectionstring/) | Die Verbindungszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen. |
| [GetSecondCommand](./getsecondcommand/) | Gibt eine zweite Befehlszeichenfolge an, die beibehalten wird, wenn PivotTable-Server-basierte Seitenfelder verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfangreichere Abfrage als command (keine WHERE-Klausel ist im Ersteren vorhanden). Basierend auf diesen 2 Befehlen (Command und ServerCommand) kann die parameter UI gefüllt und parametrisierte Abfragen erstellt werden. |
| [SetSecondCommand](./setsecondcommand/) | Gibt eine zweite Befehlszeichenfolge an, die beibehalten wird, wenn PivotTable-Server-basierte Seitenfelder verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfangreichere Abfrage als command (keine WHERE-Klausel ist im Ersteren vorhanden). Basierend auf diesen 2 Befehlen (Command und ServerCommand) kann die parameter UI gefüllt und parametrisierte Abfragen erstellt werden. |
