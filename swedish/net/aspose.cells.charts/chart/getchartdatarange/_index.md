---
title: "Chart.GetChartDataRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagrammetod. Hämtar datakällans område för diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chart/getchartdatarange/
---
## Chart.GetChartDataRange method

Hämtar diagrammets datakällintervall.

```csharp
public string GetChartDataRange()
```

### Returvärde

Datakällan.

### Anmärkningar

Stöder endast område. Om Series.Values, Name och XValues finns i ett kontinuerligt område, returneras ett område som innehåller dem.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodGetChartDataRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C4"].PutValue(60);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("=Sheet1!$B$1:$C$4", true);
            
            // Hämta och visa diagrammets dataintervall
            string dataRange = chart.GetChartDataRange();
            Console.WriteLine("Chart Data Range: " + dataRange);
            
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


