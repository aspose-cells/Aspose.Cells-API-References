---
title: "Klasse DataModelConnection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.DataModelConnection‑Klasse. Gibt eine Datenmodellverbindung an"
type: docs
url: /de/net/aspose.cells.externalconnections/datamodelconnection/
---
## DataModelConnection class

Gibt eine Datenmodellverbindung an

```csharp
public class DataModelConnection : ExternalConnection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Verwendung der Verbindung darin besteht, im Hintergrund asynchron zu aktualisieren; false, wenn die bevorzugte Verwendung der Verbindung darin besteht, im Vordergrund synchron zu aktualisieren. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/datamodelconnection/classtype/) { get; } | Ermittelt den Typ dieses [`ExternalConnection`](../externalconnection/) Objekts. |
| override [Command](../../aspose.cells.externalconnections/datamodelconnection/command/) { get; set; } | Die Zeichenkette, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen |
| override [CommandType](../../aspose.cells.externalconnections/datamodelconnection/commandtype/) { get; set; } | Gibt den Typ [`OLEDBCommandType`](../oledbcommandtype/) zurück. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Gibt die Benutzerbeschreibung für diese Verbindung an (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Ermittelt die Verbindungsdatei. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Gibt den eindeutigen Bezeichner dieser Verbindung an. (Vererbt von [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionString](../../aspose.cells.externalconnections/datamodelconnection/connectionstring/) { get; set; } | Die Verbindungsinformationszeichenkette wird verwendet, um Kontakt mit einer OLE DB- oder ODBC-Datenquelle aufzunehmen. |
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

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Collections.Generic;

    public class ExternalConnectionsClassDataModelConnectionDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();

            try
            {
                // Erstelle eine Instanz der DataModelConnection‑Klasse mittels Reflexion
                DataModelConnection connection = (DataModelConnection)System.Runtime.Serialization.FormatterServices.GetUninitializedObject(typeof(DataModelConnection));

                // Setze wesentliche Eigenschaften
                connection.Command = "SELECT * FROM Products";
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Füge die Verbindung zu den Datenverbindungen der Arbeitsmappe hinzu
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Zeige Verbindungsinformationen an
                Console.WriteLine($"Connection Type: {connection.ClassType}");
                Console.WriteLine($"Command: {connection.Command}");
                Console.WriteLine($"Command Type: {connection.CommandType}");
                Console.WriteLine($"Connection String: {connection.ConnectionString}");

                // Speichere die Arbeitsmappe
                workbook.Save("DataModelConnectionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with DataModelConnection.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DataModelConnection: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


