---
title: "Axis.IsAutomaticMajorUnit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Anger om huvudenheten för axeln tilldelas automatiskt"
type: docs
url: /sv/net/aspose.cells.charts/axis/isautomaticmajorunit/
---
## Axis.IsAutomaticMajorUnit property

Indikerar om huvudvärdet för axeln tilldelas automatiskt.

```csharp
public bool IsAutomaticMajorUnit { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMajorUnitDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Kontrollera och visa status för automatisk huvudenhet
            Console.WriteLine("IsAutomaticMajorUnit (default): " + chart.ValueAxis.IsAutomaticMajorUnit);
            
            // Inaktivera automatisk huvudenhet och ange anpassat värde
            chart.ValueAxis.IsAutomaticMajorUnit = false;
            chart.ValueAxis.MajorUnit = 5;
            Console.WriteLine("IsAutomaticMajorUnit (after change): " + chart.ValueAxis.IsAutomaticMajorUnit);
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


