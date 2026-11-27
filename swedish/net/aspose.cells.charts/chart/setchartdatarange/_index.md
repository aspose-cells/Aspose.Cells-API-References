---
title: "Chart.SetChartDataRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart‑metod. Anger dataintervall för ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

Anger dataintervall för ett diagram.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | String | Anger värden som data-serien ska plottas från |
| ärVertikal | Boolean | Anger om serien ska plottas från ett område med cellvärden radvis eller kolumnvis. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSetChartDataRangeWithStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B4"].PutValue(30);
            
            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:B4", true);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


