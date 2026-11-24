---
title: "Klasse DBConnection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.DBConnection Klasse. Gibt alle Eigenschaften an, die mit einer ODBC- oder OLE DB-externen Datenverbindung verbunden sind"
type: docs
url: /de/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Gibt alle Eigenschaften an, die mit einer externen ODBC‑ oder OLE‑DB‑Datenverbindung verbunden sind.

```csharp
public class DBConnection : ExternalConnection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Verwendung der Verbindung darin besteht, im Hintergrund asynchron zu aktualisieren; false, wenn die bevorzugte Verwendung der Verbindung darin besteht, im Vordergrund synchron zu aktualisieren. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/dbconnection/classtype/) { get; } | Ermittelt den Typ dieses [`ExternalConnection`](../externalconnection/) Objekts. |
| override [Command](../../aspose.cells.externalconnections/dbconnection/command/) { get; set; } | Die Zeichenkette, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen |
| override [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype/) { get; set; } | Gibt den OLE DB-Befehlstyp an. 1. Abfrage gibt einen Würfelnamen an 2. Abfrage gibt eine SQL-Anweisung an 3. Abfrage gibt einen Tabellennamen an 4. Abfrage gibt an, dass Standardinformationen bereitgestellt wurden, und es liegt am Anbieter, wie diese interpretiert werden. 5. Abfrage erfolgt gegen einen webbasierten List Data Provider. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Gibt die Benutzerbeschreibung für diese Verbindung an (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Ermittelt die Verbindungsdatei. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Gibt den eindeutigen Bezeichner dieser Verbindung an. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo/) { get; set; } | (**Obsolete.**) Die Verbindungsinformationszeichenkette wird verwendet, um Kontakt mit einer OLE DB- oder ODBC-Datenquelle aufzunehmen. |
| override [ConnectionString](../../aspose.cells.externalconnections/dbconnection/connectionstring/) { get; set; } | Die Verbindungsinformationszeichenkette wird verwendet, um Kontakt mit einer OLE DB- oder ODBC-Datenquelle aufzunehmen. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet wird. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Gibt die Authentifizierungsmethode an, die beim Herstellen (oder Wiederherstellen) der Verbindung verwendet wird. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Ermittelt die ID der Verbindung. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Gibt an, ob die zugehörige Arbeitsbuchverbindung gelöscht wurde. true, wenn die Verbindung gelöscht wurde; andernfalls false. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True, wenn die Verbindung zum ersten Mal nicht aktualisiert wurde; andernfalls false. Dieser Zustand kann auftreten, wenn der Benutzer die Datei speichert, bevor eine Abfrage abgeschlossen ist. (Verernt von [`ExternalConnection`](../externalconnection/).) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True, wenn die Tabellenkalkulationsanwendung versuchen soll, die Verbindung offen zu halten. Wenn false, sollte die Anwendung die Verbindung nach dem Abrufen der Informationen schließen. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Gibt den vollständigen Pfad zur externen Verbindungsdatei an, aus der diese Verbindung erstellt wurde. Wenn eine Verbindung während eines Versuchs, Daten zu aktualisieren, fehlschlägt und reconnectionMethod=1, dann versucht die Tabellenkalkulationsanwendung erneut, die Informationen aus der externen Verbindungsdatei anstelle des in der Arbeitsmappe eingebetteten Verbindungsobjekts zu verwenden. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Gibt an, ob die Tabellenkalkulationsanwendung bei einer Aktualisierung der Verbindung stets ausschließlich die Verbindungsinformationen in der externen Verbindungsdatei, die durch das Attribut odcFile angegeben ist, verwenden soll. Wenn false, dann sollte die Tabellenkalkulationsanwendung das durch das Attribut reconnectionMethod attribute(Inherited von [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Ruft [`ConnectionParameterCollection`](../connectionparametercollection/) für eine ODBC- oder Webabfrage ab. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula/) { get; } | Ruft die Definition der Power‑Query‑Formel ab. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Gibt die Anzahl der Minuten zwischen automatischen Aktualisierungen der Verbindung an. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True, wenn diese Verbindung beim Öffnen der Datei aktualisiert werden soll; andernfalls false. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True, wenn die über die Verbindung abgerufenen externen Daten zum Befüllen einer Tabelle mit der Arbeitsmappe gespeichert werden sollen; andernfalls false. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True, wenn das Passwort als Teil der Verbindungszeichenfolge gespeichert werden soll; andernfalls False. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| override [SecondCommand](../../aspose.cells.externalconnections/dbconnection/secondcommand/) { get; set; } | Gibt eine zweite Befehlszeichenfolge an, die gespeichert wird, wenn serverbasierte Seitenfelder einer PivotTable verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfangreichere Abfrage als command (es ist keine WHERE‑Klausel in ersterer enthalten). Basierend auf diesen beiden Befehlen (Command und ServerCommand) kann die Parameter‑UI gefüllt und parametrisierte Abfragen erstellt werden |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand/) { get; set; } | (**Obsolete.**) Gibt eine zweite Befehlszeichenfolge an, die gespeichert wird, wenn serverbasierte Seitenfelder einer PivotTable verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfangreichere Abfrage als command (es ist keine WHERE‑Klausel in ersterer enthalten). Basierend auf diesen beiden Befehlen (Command und ServerCommand) kann die Parameter‑UI gefüllt und parametrisierte Abfragen erstellt werden |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, direkt zu dieser Datei zu verbinden. Kann in URI- oder systemabhängiger Dateipfadnotation angegeben werden. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Liest oder setzt den Typ der externen Verbindungs‑DataSource. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Bezeichner für Single Sign On (SSO), das für die Authentifizierung zwischen einem Zwischenserver für spreadsheetML und der externen Datenquelle verwendet wird. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Liest oder setzt den Typ der externen Verbindungs‑DataSource. (Vererbt von [`ExternalConnection`](../externalconnection/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassDBConnectionDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle eine neue DBConnection‑Instanz, indem du sie zur Sammlung hinzufügst
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Grundlegende Eigenschaften festlegen
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Zeige schreibgeschützte Eigenschaften an
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                Console.WriteLine("ConnectionString: " + dbConnection.ConnectionString);
                Console.WriteLine("CommandType: " + dbConnection.CommandType);
                Console.WriteLine("Command: " + dbConnection.Command);

                // Speichere die Arbeitsmappe
                workbook.Save("DBConnectionDemo.xlsx");
                Console.WriteLine("DBConnection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DBConnection: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


