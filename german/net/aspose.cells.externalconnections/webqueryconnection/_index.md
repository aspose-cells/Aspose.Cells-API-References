---
title: "Klasse WebQueryConnection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.WebQueryConnection‑Klasse. Gibt die Eigenschaften einer Web‑Abfragequelle an. Eine Web‑Abfrage ruft Daten aus HTML‑Tabellen ab und kann außerdem HTTP‑GET‑Parameter bereitstellen, die vom Web‑Server bei der Erzeugung des HTML verarbeitet werden, indem die Parameter und Parameterelemente eingebunden werden."
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Gibt die Eigenschaften für eine Web‑Abfragequelle an. Eine Web‑Abfrage ruft Daten aus HTML‑Tabellen ab und kann außerdem HTTP‑"Get"-Parameter bereitstellen, die vom Web‑Server bei der Generierung des HTML verarbeitet werden, indem die Parameter und Parameterelemente eingebunden werden.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Verwendung der Verbindung darin besteht, im Hintergrund asynchron zu aktualisieren; false, wenn die bevorzugte Verwendung der Verbindung darin besteht, im Vordergrund synchron zu aktualisieren. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/webqueryconnection/classtype/) { get; } | Ermittelt den Typ dieses [`ExternalConnection`](../externalconnection/) Objekts. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | Der String, der den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen (geerbt von [`ExternalConnection`](../externalconnection/).) |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Gibt den OLE‑DB‑Befehlstyp an. 1. Abfrage gibt einen Würfelnamen an 2. Abfrage gibt eine SQL‑Anweisung an 3. Abfrage gibt einen Tabellennamen an 4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden, und überlässt es dem Anbieter, wie diese zu interpretieren sind. 5. Abfrage richtet sich gegen einen webbasierten List Data Provider. (geerbt von [`ExternalConnection`](../externalconnection/).) |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Gibt die Benutzerbeschreibung für diese Verbindung an (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionFile](../../aspose.cells.externalconnections/webqueryconnection/connectionfile/) { get; } | Liest die Verbindungsdatei. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Gibt den eindeutigen Bezeichner dieser Verbindung an. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | Der Verbindungszeichenfolgen-String wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet wird. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet wird. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage/) { get; set; } | (**Obsolete.**) Die URL der benutzerorientierten Webseite, die die Webabfragedaten anzeigt. Diese URL wird gespeichert, falls sourceData=\"true\" ist und die URL zu einer XML-Datei umgeleitet wurde. Dann kann die benutzerorientierte Seite in der UI angezeigt werden und die XML-Daten können im Hintergrund abgerufen werden. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage/) { get; set; } | Die URL der benutzerorientierten Webseite, die die Webabfragedaten anzeigt. Diese URL wird gespeichert, falls sourceData=\"true\" ist und die URL zu einer XML-Datei umgeleitet wurde. Dann kann die benutzerorientierte Seite in der UI angezeigt werden und die XML-Daten können im Hintergrund abgerufen werden. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat/) { get; set; } | Wie die Formatierung aus der HTML-Quelle behandelt werden soll, wenn Webabfragedaten in das Arbeitsblatt übernommen werden. Relevant, wenn sourceData True ist. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Ermittelt die ID der Verbindung. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive/) { get; set; } | Flag, das angibt, ob aufeinanderfolgende Trennzeichen als ein einzelnes Trennzeichen behandelt werden sollen. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Gibt an, ob die zugehörige Arbeitsbuchverbindung gelöscht wurde. true, wenn die Verbindung gelöscht wurde; andernfalls false. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables/) { get; set; } | Flag, das angibt, ob Webabfragen nur mit HTML-Tabellen funktionieren sollen. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True, wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage abgeschlossen ist. (Verernt von [`ExternalConnection`](../externalconnection/).) |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre/) { get; set; } | Flag, das angibt, ob Daten, die in HTML‑PRE‑Tags auf der Webseite enthalten sind, beim Importieren der Seite in eine Abfragetabelle in Spalten aufgeteilt werden. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings/) { get; set; } | Flag, das angibt, ob alle Tabellen innerhalb eines PRE‑Blocks mit denselben Breiteneinstellungen wie die erste Zeile geparst werden sollen. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates/) { get; set; } | Flag, das angibt, ob Daten als Text statt als Datum in Zellen des Arbeitsblatts importiert werden sollen. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000/) { get; set; } | Dieses Flag dient der Abwärtskompatibilität mit älteren vorhandenen Tabellenkalkulationsdateien und ist auf true gesetzt, wenn diese Webabfrage in einer Tabellenkalkulationsanwendung, die neuer oder gleich Microsoft Excel 2000 ist, aktualisiert wurde. Dies ist ein optionales Attribut, das ignoriert werden kann. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97/) { get; set; } | Dieses Flag dient der Abwärtskompatibilität mit älteren vorhandenen Tabellenkalkulationsdateien und ist auf true gesetzt, wenn diese Webabfrage in Microsoft Excel 97 erstellt wurde. Dies ist ein optionales Attribut, das ignoriert werden kann. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml/) { get; set; } | true, wenn die Webabfragequelle XML (statt HTML) ist, andernfalls false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/) { get; set; } | Flag, das angibt, dass XML-Quelldaten importiert werden sollen anstelle der HTML‑Tabelle selbst. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True, wenn die Tabellenkalkulationsanwendung versuchen soll, die Verbindung offen zu halten. Wenn false, sollte die Anwendung die Verbindung nach dem Abrufen der Informationen schließen. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung während eines Versuchs, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1, dann versucht die Tabellenkalkulationsanwendung erneut, die Informationen aus der externen Verbindungsdatei anstelle des in der Arbeitsmappe eingebetteten Verbindungsobjekts zu verwenden. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Gibt an, ob die Tabellenkalkulationsanwendung bei einer Aktualisierung der Verbindung stets ausschließlich die Verbindungsinformationen in der externen Verbindungsdatei, die durch das Attribut odcFile angegeben ist, verwenden soll. Wenn false, dann sollte die Tabellenkalkulationsanwendung das durch das Attribut reconnectionMethod attribute(Inherited von [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Ruft [`ConnectionParameterCollection`](../connectionparametercollection/) für eine ODBC- oder Webabfrage ab. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post/) { get; set; } | Gibt die Zeichenfolge zurück oder legt sie fest, die mit der POST‑Methode zum Senden von Daten an einen Webserver verwendet wird, um Daten aus einer Webabfrage zurückzugeben. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Liest die Definition der Power‑Query‑Formel. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls false. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit der Arbeitsmappe gespeichert werden sollen; andernfalls false. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls False. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Gibt eine zweite Befehls‑Textzeichenfolge an, die gespeichert wird, wenn serverbasierte Seitenfelder einer PivotTable verwendet werden. Für ODBC‑Verbindungen ist serverCommand in der Regel eine umfassendere Abfrage als command (bei ersterer fehlt die WHERE‑Klausel). Auf Basis dieser beiden Befehle (Command und ServerCommand) kann die Parameter‑UI gefüllt und parametrisierte Abfragen erstellt werden (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, direkt zu dieser Datei zu verbinden. Kann in URI- oder systemabhängiger Dateipfadnotation angegeben werden. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Liest oder setzt den Typ der externen Verbindungs‑DataSource. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Bezeichner für Single Sign On (SSO), das für die Authentifizierung zwischen einem Zwischenserver für spreadsheetML und der externen Datenquelle verwendet wird. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Liest oder setzt den Typ der externen Verbindungs‑DataSource. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url/) { get; set; } | URL, die zum Aktualisieren externer Daten verwendet wird. |

### Beispiele

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
                // Webabfrageverbindung über die Sammlung erstellen
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

### Siehe auch

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


