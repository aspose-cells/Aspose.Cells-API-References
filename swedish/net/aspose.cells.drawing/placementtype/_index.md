---
title: "Enum PlacementType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.PlacementType-enum. Representerar hur ritobjektet är fäst vid cellerna under det"
type: docs
url: /sv/net/aspose.cells.drawing/placementtype/
---
## PlacementType enumeration

Representerar hur ritobjektet är fäst vid cellerna under det.

```csharp
public enum PlacementType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| FreeFloating | `0` | Flytta inte eller ändra storlek med celler. |
| Move | `1` | Flytta men ändra inte storlek med celler. |
| MoveAndSize | `2` | Flytta och ändra storlek med celler. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class PlacementTypeDemo
    {
        public static void PlacementTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Ange placeringstypen för diagrammet
            chart.Placement = PlacementType.MoveAndSize;

            // Skriv ut placeringstypen
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // Spara arbetsboken
            workbook.Save("PlacementTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


