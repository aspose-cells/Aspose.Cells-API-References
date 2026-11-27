---
title: "LegendEntry.IsDeleted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LegendEntry egenskap. Hämtar och anger om legendposten är raderad"
type: docs
url: /sv/net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Hämtar och anger om legendposten är borttagen.

```csharp
public bool IsDeleted { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Hämta den första legendposten
            LegendEntry legendEntry = chart.Legend.LegendEntries[0];

            // Demonstrera egenskapen IsDeleted
            Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
            
            // Radera legendposten
            legendEntry.IsDeleted = true;
            Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);

            // Återställ legendposten
            legendEntry.IsDeleted = false;
            Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);

            // Spara arbetsboken
            workbook.Save("LegendEntryIsDeletedDemo.xlsx");
        }
    }
}
```

### Se även

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


