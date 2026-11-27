---
title: "Axis.TickLabelPosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar positionen för tick‑etikett på den angivna axeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/ticklabelposition/
---
## Axis.TickLabelPosition property

Anger positionen för tick‑etikett på den angivna axeln.

```csharp
public TickLabelPositionType TickLabelPosition { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelPositionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ange tick‑etikettens position
            chart.CategoryAxis.TickLabelPosition = TickLabelPositionType.Low;
            
            // Spara arbetsboken
            workbook.Save("AxisPropertyTickLabelPositionDemo_out.xlsx");
        }
    }
}
```

### Se även

* enum [TickLabelPositionType](../../ticklabelpositiontype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


