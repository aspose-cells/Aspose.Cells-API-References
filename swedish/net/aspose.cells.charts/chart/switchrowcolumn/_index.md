---
title: "Chart.SwitchRowColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagrammetod. Växlar rad/kolumn"
type: docs
url: /sv/net/aspose.cells.charts/chart/switchrowcolumn/
---
## Chart.SwitchRowColumn method

Byter rad/kolumn.

```csharp
public bool SwitchRowColumn()
```

### Returvärde

False betyder att växling av rad/kolumn misslyckas.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSwitchRowColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C4"].PutValue(350);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:C4", true);
            
            // Visa originalvärden för serierna
            Console.WriteLine("Before SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Växla rad/kolumn
            chart.SwitchRowColumn();
            
            // Visa serievärden efter växling
            Console.WriteLine("\nAfter SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Spara arbetsboken
            workbook.Save("SwitchRowColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


