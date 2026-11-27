---
title: "Axis.IsAutomaticMaxValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Anger om maxvärdet tilldelas automatiskt"
type: docs
url: /sv/net/aspose.cells.charts/axis/isautomaticmaxvalue/
---
## Axis.IsAutomaticMaxValue property

Indikerar om maxvärdet tilldelas automatiskt.

```csharp
public bool IsAutomaticMaxValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMaxValueDemo
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
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta värdeaxeln
            Axis valueAxis = chart.ValueAxis;

            // Demonstrera egenskapen IsAutomaticMaxValue
            Console.WriteLine("Initial IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("Initial MaxValue: " + valueAxis.MaxValue);

            // Inaktivera automatiskt maxvärde och ange anpassat värde
            valueAxis.IsAutomaticMaxValue = false;
            valueAxis.MaxValue = 40;
            Console.WriteLine("After change - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After change - MaxValue: " + valueAxis.MaxValue);

            // Aktivera automatiskt maxvärde igen
            valueAxis.IsAutomaticMaxValue = true;
            Console.WriteLine("After re-enabling - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After re-enabling - MaxValue: " + valueAxis.MaxValue);

            // Spara arbetsboken
            workbook.Save("AxisPropertyIsAutomaticMaxValueDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


