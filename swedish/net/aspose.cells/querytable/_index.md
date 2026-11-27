---
title: "Klass QueryTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.QueryTable‑klass. Representerar QueryTable‑information"
type: docs
url: /sv/net/aspose.cells/querytable/
---
## QueryTable class

Representerar QueryTable‑information.

```csharp
public class QueryTable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Returnerar eller anger AdjustColumnWidth för objektet. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Hämtar anslutnings‑id för frågetabellen. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | Hämtar den relaterade externa anslutningen. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Hämtar namnet på querytable. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Returnerar eller anger PreserveFormatting för objektet. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Hämtar intervallet för resultatet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassQueryTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att skapa en frågetabell (simulerar externa data)
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Kontrollera om det finns några frågetabeller i kalkylbladet
            if (worksheet.QueryTables.Count > 0)
            {
                // Hämta den första frågetabellen
                QueryTable qt = worksheet.QueryTables[0];
                
                // Visa egenskaper för frågetabellen
                Console.WriteLine("Query Table Name: " + qt.Name);
                Console.WriteLine("Connection ID: " + qt.ConnectionId);
                Console.WriteLine("Result Range: " + qt.ResultRange.Address);
                Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
                Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
                
                // Ändra några egenskaper
                qt.PreserveFormatting = true;
                qt.AdjustColumnWidth = false;
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


