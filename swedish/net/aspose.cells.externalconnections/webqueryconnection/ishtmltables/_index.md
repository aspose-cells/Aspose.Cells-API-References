---
title: "WebQueryConnection.IsHtmlTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. Flagga som indikerar om webbfrågor endast ska fungera på HTML‑tabeller"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/ishtmltables/
---
## WebQueryConnection.IsHtmlTables property

Flagga som anger om webbfrågor endast ska fungera på HTML-tabeller.

```csharp
public bool IsHtmlTables { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsHtmlTablesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Skapa webbfrågeanslutning via samlingsindexer
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

                Console.WriteLine("Initial IsHtmlTables: " + connection.IsHtmlTables);
                
                connection.IsHtmlTables = true;
                Console.WriteLine("Updated IsHtmlTables: " + connection.IsHtmlTables);

                workbook.Save("IsHtmlTablesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


