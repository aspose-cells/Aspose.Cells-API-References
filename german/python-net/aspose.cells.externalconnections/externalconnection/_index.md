---
title: ExternalConnection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 50
url: /de/python-net/aspose.cells.externalconnections/externalconnection/
is_root: false
---
##  ExternalConnection Klasse
Gibt eine externe Datenverbindung an



Der Typ ExternalConnection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [id](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/id) | Ruft die ID der Verbindung ab.|
| [power_query_formula](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/power_query_formula) | Ruft die Definition der Leistungsabfrageformel ab.|
| [type](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/type) | Ruft den DataSource-Typ der externen Verbindung ab oder legt diesen fest.|
| [source_file](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/source_file) | Wird verwendet, wenn die externe Datenquelle dateibasiert ist.<br/> source fehlschlägt, versucht die Tabellenkalkulationsanwendung, eine direkte Verbindung zu dieser Datei herzustellen.<br/> ausgedrückt in URI oder systemspezifischer Dateipfadnotation.|
| [sso_id](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/sso_id) | Bezeichner für Single Sign On (SSO), der für die Authentifizierung zwischen einem Intermediate verwendet wird<br/> SpreadsheetML-Server und die externe Datenquelle.|
| [save_password](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/save_password) | True, wenn das Kennwort als Teil der Verbindungszeichenfolge gespeichert werden soll, andernfalls False.|
| [save_data](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/save_data) | True, wenn die über die Verbindung abgerufenen externen Daten zum Füllen einer Tabelle gespeichert werden sollen<br/> mit der Arbeitsmappe, andernfalls false.|
| [refresh_on_load](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/refresh_on_load) | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll;|
| [reconnection_method_type](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/reconnection_method_type) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.<br/>Der Standardwert ist ReConnectionMethodType.Required.|
| [reconnection_method](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/reconnection_method) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.<br/>Der Standardwert ist ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/only_use_connection_file) | Gibt an, ob die Tabellenkalkulationsanwendung immer und nur die verwenden soll<br/> Verbindungsinformationen in der externen Verbindungsdatei, die durch das Attribut odcFile angegeben wird<br/> wenn die Verbindung aktualisiert wird. Wenn falsch, dann die Tabellenkalkulationsanwendung<br/> sollte dem durch das Attribut reconnectionMethod angegebenen Verfahren folgen|
| [odc_file](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/odc_file) | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, von der diese Verbindung stammt<br/> Wenn eine Verbindung beim Versuch, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1,<br/> dann versucht die Tabellenkalkulationsanwendung erneut, Informationen aus der externen Verbindungsdatei zu verwenden<br/> anstelle des in die Arbeitsmappe eingebetteten Verbindungsobjekts.|
| [is_new](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/is_new) | True, wenn die Verbindung nicht zum ersten Mal aktualisiert wurde, andernfalls false.<br/> Dieser Zustand kann eintreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage die Rückgabe beendet hat.|
| [name](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/name) | Gibt den Namen der Verbindung an.|
| [keep_alive](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/keep_alive) | True, wenn das Tabellenkalkulationsprogramm Anstrengungen unternehmen soll, um die Verbindung aufrechtzuerhalten<br/>open. Bei false sollte die Anwendung die Verbindung nach dem Abrufen von schließen<br/> Information.|
| [refresh_internal](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/refresh_internal) | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an.|
| [connection_id](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/connection_id) | Gibt die eindeutige Kennung dieser Verbindung an.|
| [connection_description](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/connection_description) | Gibt die Benutzerbeschreibung für diese Verbindung an|
| [is_deleted](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/is_deleted) |Gibt an, ob die zugeordnete Arbeitsmappenverbindung gelöscht wurde. wahr, wenn die<br/> andernfalls falsch.|
| [credentials_method_type](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/credentials_method_type) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.|
| [credentials](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/credentials) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.|
| [background_refresh](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/background_refresh) | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann.<br/>true, wenn die bevorzugte Verwendung der Verbindung die asynchrone Aktualisierung im Hintergrund ist;<br/> false, wenn die bevorzugte Verwendung der Verbindung die synchrone Aktualisierung im Vordergrund ist.|
| [parameters](/cells/de/python-net/aspose.cells.externalconnections/externalconnection/parameters) | Ruft [ConnectionParameterCollection](/cells/de/python-net/aspose.cells.externalconnections/connectionparametercollection) für eine ODBC- oder Webabfrage ab.|



###  Siehe auch
* Modul [aspose.cells.externalconnections](..)
* Klasse [ConnectionParameterCollection](/cells/de/python-net/aspose.cells.externalconnections/connectionparametercollection)
