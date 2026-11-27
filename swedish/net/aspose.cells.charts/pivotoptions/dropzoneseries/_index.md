---
title: "PivotOptions.DropZoneSeries"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotOptions-egenskap. Anger om en kontroll för varje PivotTable-fält på PivotTable‑kolumnaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true"
type: docs
url: /sv/net/aspose.cells.charts/pivotoptions/dropzoneseries/
---
## PivotOptions.DropZoneSeries property

Anger om en kontroll för varje PivotTable‑fält på kolumnaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true.

```csharp
public bool DropZoneSeries { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneSeriesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett arbetsblad och hämta det första bladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(7);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A1:B4", true);
            
            // Hämta pivotalternativ från diagrammet
            PivotOptions options = chart.PivotOptions;
            
            // Demonstrera egenskapen DropZoneSeries
            Console.WriteLine("Original DropZoneSeries value: " + options.DropZoneSeries);
            options.DropZoneSeries = true;
            Console.WriteLine("Modified DropZoneSeries value: " + options.DropZoneSeries);
            
            // Spara arbetsboken
            workbook.Save("PivotOptionsPropertyDropZoneSeriesDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


