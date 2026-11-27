---
title: "QueryTable.AdjustColumnWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "QueryTable-egenskap. Returnerar eller anger AdjustColumnWidth för objektet"
type: docs
url: /sv/net/aspose.cells/querytable/adjustcolumnwidth/
---
## QueryTable.AdjustColumnWidth property

Returnerar eller anger AdjustColumnWidth för objektet.

```csharp
public bool AdjustColumnWidth { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyAdjustColumnWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med varierande kolumnbredder
            worksheet.Cells["A1"].PutValue("Narrow Column");
            worksheet.Cells["B1"].PutValue("Wide Column Data");
            worksheet.Cells["A2"].PutValue("Short");
            worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");

            // Ställ in kolumnbredder manuellt
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data

            // Skapa en frågetabell (simulerad eftersom faktisk skapning kräver extern datakälla)
            QueryTable queryTable = worksheet.QueryTables[0];

            // Visa aktuellt värde för AdjustColumnWidth
            Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);

            // Ställ in AdjustColumnWidth till true och demonstrera effekten
            queryTable.AdjustColumnWidth = true;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
            Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");

            // Simulera uppdatering av frågetabellen (skulle normalt justera kolumnbredder)
            // I ett verkligt scenario skulle detta ske när frågetabellen uppdaterar sina data
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
            Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));

            // Ställ in AdjustColumnWidth till false och demonstrera effekten
            queryTable.AdjustColumnWidth = false;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);

            // Simulera uppdatering igen (skulle nu bevara ursprungliga kolumnbredder)
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
            Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));

            // Spara arbetsboken
            workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


