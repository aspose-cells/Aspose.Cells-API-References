---
title: WebQueryConnection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---
##  WebQueryConnection Klasse
 Gibt die Eigenschaften für eine Webabfragequelle an. Eine Webabfrage ruft Daten aus HTML-Tabellen ab,
 und kann auch HTTP-"Get"-Parameter liefern, die vom Webserver beim Generieren der HTML verarbeitet werden sollen
einschließlich der Parameter und Parameterelemente.



**Nachlass:** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/de/python-net/aspose.cells.externalconnections/externalconnection)



Der Typ WebQueryConnection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [id](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/id) | Ruft die ID der Verbindung ab.|
| [power_query_formula](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) | Ruft die Definition der Leistungsabfrageformel ab.|
| [type](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/type) | Ruft den DataSource-Typ der externen Verbindung ab oder legt diesen fest.|
| [source_file](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) | Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Bei einer Verbindung zu solchen Daten<br/> source fehlschlägt, versucht die Tabellenkalkulationsanwendung, eine direkte Verbindung zu dieser Datei herzustellen. Vielleicht<br/> ausgedrückt in URI oder systemspezifischer Dateipfadnotation.|
| [sso_id](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) | Bezeichner für Single Sign On (SSO), der für die Authentifizierung zwischen einem Intermediate verwendet wird<br/>SpreadsheetML-Server und die externe Datenquelle.|
| [save_password](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) |True, wenn das Kennwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls falsch.|
| [save_data](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) | True, wenn die über die Verbindung abgerufenen externen Daten zum Füllen einer Tabelle gespeichert werden sollen<br/> mit dem Arbeitsbuch; andernfalls falsch.|
| [refresh_on_load](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls falsch.|
| [reconnection_method_type](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.<br/> Der Standardwert ist ReConnectionMethodType.Required.|
| [reconnection_method](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.<br/> Der Standardwert ist ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) | Gibt an, ob die Tabellenkalkulationsanwendung immer und nur die verwenden soll<br/> Verbindungsinformationen in der externen Verbindungsdatei, die durch das Attribut odcFile angegeben wird<br/> wenn die Verbindung aktualisiert wird. Wenn falsch, dann die Tabellenkalkulationsanwendung<br/> sollte dem durch das Attribut reconnectionMethod angegebenen Verfahren folgen|
| [odc_file](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, von der diese Verbindung stammt<br/> erstellt. Wenn eine Verbindung beim Versuch, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1,<br/> dann versucht die Tabellenkalkulationsanwendung erneut, Informationen aus der externen Verbindungsdatei zu verwenden<br/> anstelle des in die Arbeitsmappe eingebetteten Verbindungsobjekts.|
| [is_new](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) | True, wenn die Verbindung nicht zum ersten Mal aktualisiert wurde; andernfalls falsch.<br/> Dieser Zustand kann eintreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage die Rückgabe beendet hat.|
| [name](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/name) | Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben.|
| [keep_alive](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) | True, wenn das Tabellenkalkulationsprogramm Anstrengungen unternehmen soll, um die Verbindung aufrechtzuerhalten<br/> offen. Bei „false“ sollte die Anwendung die Verbindung nach dem Abrufen von schließen<br/> Information.|
| [refresh_internal](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an.|
| [connection_id](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) | Gibt den eindeutigen Bezeichner dieser Verbindung an.|
| [connection_description](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) | Gibt die Benutzerbeschreibung für diese Verbindung an|
| [is_deleted](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) | Gibt an, ob die zugehörige Arbeitsmappenverbindung gelöscht wurde. wahr, wenn die<br/> Verbindung wurde gelöscht; andernfalls falsch.|
| [credentials_method_type](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.|
| [credentials](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll.|
| [background_refresh](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann.<br/> true, wenn die bevorzugte Verwendung der Verbindung die asynchrone Aktualisierung im Hintergrund ist;<br/>false, wenn die bevorzugte Verwendung der Verbindung die synchrone Aktualisierung im Vordergrund ist.|
| [parameters](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) | Ruft [ConnectionParameterCollection](/cells/de/python-net/aspose.cells.externalconnections/connectionparametercollection) für eine ODBC- oder Webabfrage ab.|
| [is_xml](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) | true, wenn die Quelle der Webabfrage XML ist (gegenüber HTML), andernfalls false.|
| [is_xl97](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) | Dieses Flag dient der Abwärtskompatibilität mit älteren vorhandenen Tabellenkalkulationsdateien und ist gesetzt<br/>auf „true“, wenn diese Webabfrage in Microsoft Excel 97 erstellt wurde.<br/> Dies ist ein optionales Attribut, das ignoriert werden kann.|
| [is_xl2000](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) | Dieses Flag dient der Abwärtskompatibilität mit älteren vorhandenen Tabellenkalkulationsdateien und ist gesetzt<br/>auf „true“, wenn diese Webabfrage in einer Tabellenkalkulationsanwendung aktualisiert wurde, die neuer als oder gleich ist<br/>an Microsoft Excel 2000.<br/> Dies ist ein optionales Attribut, das ignoriert werden kann.|
| [url](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/url) | URL zum Aktualisieren externer Daten.|
| [is_text_dates](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) | Flag, das angibt, ob Datumsangaben als Text und nicht als Datumsangaben in Zellen im Arbeitsblatt importiert werden sollen.|
| [is_xml_source_data](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) | Flag, das angibt, dass XML-Quelldaten anstelle der Tabelle HTML selbst importiert werden sollen.|
| [post](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/post) | Gibt die Zeichenfolge zurück oder legt sie fest, die mit der post-Methode zum Eingeben von Daten in einen Webserver verwendet wird<br/> um Daten aus einer Webabfrage zurückzugeben.|
| [is_parse_pre](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) |Flag, das angibt, ob Daten innerhalb von HTML PRE-Tags in der Webseite enthalten sind<br/> in Spalten geparst, wenn Sie die Seite in eine Abfragetabelle importieren.|
| [is_html_tables](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) | Flag, das angibt, ob Webabfragen nur auf HTML-Tabellen funktionieren sollen.|
| [html_format](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) | Umgang mit der Formatierung aus der Quelle HTML beim Einbringen von Webabfragedaten in die<br/> Arbeitsblatt. Relevant, wenn sourceData True ist.|
| [is_same_settings](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) | Flag, das angibt, ob alle Tabellen innerhalb eines PRE-Blocks mit denselben Breiteneinstellungen analysiert werden sollen<br/> als erste Reihe.|
| [edit_web_page](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) | Die URL der benutzerseitigen Webseite, die die Webabfragedaten anzeigt. Diese URL wird beibehalten<br/>für den Fall, dass sourceData="true" und url umgeleitet wurden, um auf eine XML-Datei zu verweisen.<br/>Anschließend kann die benutzerseitige Seite in der Benutzeroberfläche angezeigt und die XML-Daten abgerufen werden<br/> hinter den Kulissen.|
| [edit_page](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) | Die URL der benutzerseitigen Webseite, die die Webabfragedaten anzeigt. Diese URL wird beibehalten<br/>für den Fall, dass sourceData="true" und url umgeleitet wurden, um auf eine XML-Datei zu verweisen.<br/>Anschließend kann die benutzerseitige Seite in der Benutzeroberfläche angezeigt und die XML-Daten abgerufen werden<br/> hinter den Kulissen.|
| [is_consecutive](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) | Flag, das angibt, ob aufeinanderfolgende Trennzeichen als nur ein Trennzeichen behandelt werden sollen.|



###  Siehe auch
* Modul [aspose.cells.externalconnections](..)
* Klasse [ConnectionParameterCollection](/cells/de/python-net/aspose.cells.externalconnections/connectionparametercollection)
* Klasse [ExternalConnection](/cells/de/python-net/aspose.cells.externalconnections/externalconnection)
* Klasse [WebQueryConnection](/cells/de/python-net/aspose.cells.externalconnections/webqueryconnection)
