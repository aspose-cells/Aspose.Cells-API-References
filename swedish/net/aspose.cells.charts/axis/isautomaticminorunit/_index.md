---
title: "Axis.IsAutomaticMinorUnit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis property. Anger om den mindre enheten för axeln tilldelas automatiskt"
type: docs
url: /sv/net/aspose.cells.charts/axis/isautomaticminorunit/
---
## Axis.IsAutomaticMinorUnit property

Indikerar om delvärdet för axeln tilldelas automatiskt.

```csharp
public bool IsAutomaticMinorUnit { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinorUnitDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
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
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Hämta värdeaxeln
            Axis valueAxis = chart.ValueAxis;

            // Demonstrera IsAutomaticMinorUnit-egenskapen
            Console.WriteLine("Initial IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            
            // Ställ in mindre enhet manuellt
            valueAxis.IsAutomaticMinorUnit = false;
            valueAxis.MinorUnit = 2;
            Console.WriteLine("After setting manually - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            Console.WriteLine("MinorUnit: " + valueAxis.MinorUnit);

            // Ställ tillbaka till automatiskt
            valueAxis.IsAutomaticMinorUnit = true;
            Console.WriteLine("After setting automatic - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);

            // Spara arbetsboken
            workbook.Save("AxisPropertyIsAutomaticMinorUnitDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


