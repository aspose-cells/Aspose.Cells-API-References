---
title: "WebQueryConnection.Url"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebQueryConnection property. URL, die zum Aktualisieren externer Daten verwendet wird"
type: docs
url: /de/net/aspose.cells.externalconnections/webqueryconnection/url/
---
## WebQueryConnection.Url property

URL, die zum Aktualisieren externer Daten verwendet wird.

```csharp
public string Url { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyUrlDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine WebQueryConnection, indem du sie zur Sammlung hinzufügst
            // Die Sammlung wird wahrscheinlich das Verbindungsobjekt erstellen und zurückgeben
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

            // Setze die anfängliche URL für die Webabfrage
            connection.Url = "https://example.com/data.html";
            Console.WriteLine("Initial URL: " + connection.Url);

            // Ändere die URL zu einer anderen Quelle
            connection.Url = "https://example.com/updated-data.xml";
            Console.WriteLine("Updated URL: " + connection.Url);

            // Konfiguriere die Verbindung, um XML-Daten zu parsen
            connection.IsXml = true;

            // Aktualisiere die Datenverbindung (würde normalerweise Daten von der URL abrufen)
            // Hinweis: Echter Webzugriff würde Netzwerkverbindung erfordern
            // workbook.RefreshAllConnections();

            // Speichere die Arbeitsmappe mit der WebQueryConnection
            workbook.Save("WebQueryConnectionUrlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


