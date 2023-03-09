---
title: DBConnection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells.externalconnections/dbconnection/
is_root: false
---
##  DBConnection Klasse
Gibt alle Eigenschaften an, die einer externen ODBC- oder OLE DB-Datenverbindung zugeordnet sind.



**Nachlass:** [DBConnection](/cells/python-net/aspose.cells.externalconnections/dbconnection) → 
[ExternalConnection](/cells/de/python-net/aspose.cells.externalconnections/externalconnection)



Der Typ DBConnection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [id](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/id) | Ruft die ID der Verbindung ab.|
| [power_query_formula](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/power_query_formula) | Ruft die Definition der Leistungsabfrageformel ab.|
| [type](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/type) | Ruft den DataSource-Typ der externen Verbindung ab oder legt diesen fest.|
| [source_file](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/source_file) | Wird verwendet, wenn die externe Datenquelle dateibasiert ist.<br/> source fehlschlägt, versucht die Tabellenkalkulationsanwendung, eine direkte Verbindung zu dieser Datei herzustellen.<br/> ausgedrückt in URI oder systemspezifischer Dateipfadnotation.|
| [sso_id](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/sso_id) | Bezeichner für Single Sign On (SSO), der für die Authentifizierung zwischen einem Intermediate verwendet wird<br/> SpreadsheetML-Server und die externe Datenquelle.|
| [save_password](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/save_password) | True, wenn das Kennwort als Teil der Verbindungszeichenfolge gespeichert werden soll, andernfalls False.|
| [save_data](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/save_data) | True, wenn die über die Verbindung abgerufenen externen Daten zum Füllen einer Tabelle gespeichert werden sollen<br/> mit der Arbeitsmappe, andernfalls false.|
| [refresh_on_load](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/refresh_on_load) | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll;|
| [reconnection_method_type](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method_type) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.<br/>Der Standardwert ist ReConnectionMethodType.Required.|
| [reconnection_method](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.<br/>Der Standardwert ist ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/only_use_connection_file) | Gibt an, ob die Tabellenkalkulationsanwendung immer und nur die verwenden soll<br/> Verbindungsinformationen in der externen Verbindungsdatei, die durch das Attribut odcFile angegeben wird<br/> wenn die Verbindung aktualisiert wird. Wenn falsch, dann die Tabellenkalkulationsanwendung<br/> sollte dem durch das Attribut reconnectionMethod angegebenen Verfahren folgen|
| [odc_file](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/odc_file) | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, von der diese Verbindung stammt<br/> Wenn eine Verbindung beim Versuch, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1,<br/> dann versucht die Tabellenkalkulationsanwendung erneut, Informationen aus der externen Verbindungsdatei zu verwenden<br/> anstelle des in die Arbeitsmappe eingebetteten Verbindungsobjekts.|
| [is_new](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/is_new) | True, wenn die Verbindung nicht zum ersten Mal aktualisiert wurde, andernfalls false.<br/> Dieser Zustand kann eintreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage die Rückgabe beendet hat.|
| [name](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/name) | Gibt den Namen der Verbindung an.|
| [keep_alive](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/keep_alive) | True, wenn das Tabellenkalkulationsprogramm Anstrengungen unternehmen soll, um die Verbindung aufrechtzuerhalten<br/>open. Bei false sollte die Anwendung die Verbindung nach dem Abrufen von schließen<br/> Information.|
| [refresh_internal](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/refresh_internal) | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an.|
| [connection_id](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/connection_id) | Gibt die eindeutige Kennung dieser Verbindung an.|
| [connection_description](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/connection_description) | Gibt die Benutzerbeschreibung für diese Verbindung an|
| [is_deleted](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/is_deleted) |Gibt an, ob die zugeordnete Arbeitsmappenverbindung gelöscht wurde. wahr, wenn die<br/> andernfalls falsch.|
| [credentials_method_type](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/credentials_method_type) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.|
| [credentials](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/credentials) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.|
| [background_refresh](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/background_refresh) | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann.<br/>true, wenn die bevorzugte Verwendung der Verbindung die asynchrone Aktualisierung im Hintergrund ist;<br/> false, wenn die bevorzugte Verwendung der Verbindung die synchrone Aktualisierung im Vordergrund ist.|
| [parameters](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/parameters) | Ruft [ConnectionParameterCollection](/cells/de/python-net/aspose.cells.externalconnections/connectionparametercollection) für eine ODBC- oder Webabfrage ab.|
| [connection_info](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/connection_info) | Die Verbindungsinformationszeichenfolge wird verwendet, um Kontakt mit einer OLE DB- oder ODBC-Datenquelle herzustellen.|
| [command_type](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/command_type) | Gibt den OLE DB-Befehlstyp an.<br/>1. Die Abfrage gibt einen Cube-Namen an<br/>2. Query gibt eine SQL-Anweisung an<br/>3. Abfrage gibt einen Tabellennamen an<br/>4. Die Abfrage gibt an, dass Standardinformationen angegeben wurden, und es dem Anbieter überlassen ist, wie er interpretiert.<br/> 5. Die Abfrage erfolgt gegen einen webbasierten Listendatenanbieter.|
| [command](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/command) | Die Zeichenfolge, die den Datenbankbefehl enthält, der an den Datenanbieter API übergeben werden soll<br/> mit der externen Quelle interagieren, um Daten abzurufen|
| [sever_command](/cells/de/python-net/aspose.cells.externalconnections/dbconnection/sever_command) |Gibt eine zweite Befehlstextzeichenfolge an, die beibehalten wird, wenn PivotTable serverbasiert ist<br/> Seitenfelder werden verwendet.<br/> Für ODBC-Verbindungen ist serverCommand normalerweise eine breitere Abfrage als Befehl (Nr<br/>WHERE-Klausel ist in der ersteren vorhanden).<br/> Die Parameter-UI kann ausgefüllt und parametrisierte Abfragen erstellt werden|



###  Siehe auch
* Modul [aspose.cells.externalconnections](..)
* Klasse [ConnectionParameterCollection](/cells/de/python-net/aspose.cells.externalconnections/connectionparametercollection)
* Klasse [DBConnection](/cells/de/python-net/aspose.cells.externalconnections/dbconnection)
* Klasse [ExternalConnection](/cells/de/python-net/aspose.cells.externalconnections/externalconnection)
