---
title: ExternalConnection
second_title: Aspose.Cells für .NET-API-Referenz
description: Gibt eine externe Datenverbindung an
type: docs
weight: 3290
url: /de/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Gibt eine externe Datenverbindung an

```csharp
public abstract class ExternalConnection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Verwendung der Verbindung die asynchrone Aktualisierung im Hintergrund ist; false, wenn die bevorzugte Verwendung der Verbindung die synchrone Aktualisierung im Vordergrund ist. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Gibt die Benutzerbeschreibung für diese Verbindung an |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Gibt die eindeutige Kennung dieser Verbindung an. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet werden soll. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Ruft die ID der Verbindung ab. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Gibt an, ob die zugehörige Arbeitsmappenverbindung gelöscht wurde. wahr, wenn die -Verbindung gelöscht wurde; andernfalls falsch. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | True, wenn die Verbindung nicht zum ersten Mal aktualisiert wurde; andernfalls falsch. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage die Rückgabe beendet hat. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Wahr, wenn das Tabellenkalkulationsprogramm Anstrengungen unternehmen soll, um die Verbindung offen zu halten. Wenn falsch, sollte die Anwendung die Verbindung nach dem Abrufen der -Informationen schließen. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung beim Versuch, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1, , versucht die Tabellenkalkulationsanwendung erneut, Informationen aus der externen Verbindungsdatei anstelle des in die Arbeitsmappe eingebetteten Verbindungsobjekts zu verwenden. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Gibt an, ob die Tabellenkalkulationsanwendung immer und nur die -Verbindungsinformationen in der externen Verbindungsdatei verwenden soll, die durch das odcFile-Attribut angegeben wird, wenn die Verbindung aktualisiert wird. Wenn falsch, sollte die Tabellenkalkulationsanwendung dem durch das reconnectionMethod-Attribut angegebenen Verfahren folgen. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | erhält[`ConnectionParameterCollection`](../connectionparametercollection) für eine ODBC- oder Webabfrage. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Ruft die Definition der Leistungsabfrageformel ab. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls falsch. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | True, wenn die externen Daten, die über die Verbindung abgerufen werden, um eine Tabelle zu füllen, zusammen mit der Arbeitsmappe gespeichert werden sollen ; andernfalls falsch. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls falsch. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, eine direkte Verbindung zu dieser Datei herzustellen. Kann sein, ausgedrückt in URI oder systemspezifischer Dateipfadnotation. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Bezeichner für Single Sign On (SSO), der für die Authentifizierung zwischen einem zwischengeschalteten SpreadsheetML-Server und der externen Datenquelle verwendet wird. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Ruft den DataSource-Typ der externen Verbindung ab oder legt ihn fest. |

### Siehe auch

* namensraum [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
