---
title: "Chart.GetActualSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-metod. Hämtar diagrammets faktiska storlek i pixelenheter."
type: docs
url: /sv/net/aspose.cells.charts/chart/getactualsize/
---
## Chart.GetActualSize method

Hämtar diagrammets faktiska storlek i pixelenheter.

```csharp
public int[] GetActualSize()
```

### Returvärde

Faktisk storlek i en array (bredd och höjd). [0] är bredd; [1] är höjd.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodGetActualSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
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
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:B4", true);
            
            try
            {
                // Anropa GetActualSize-metoden.
                int[] actualSize = chart.GetActualSize();
                
                // Visa resultatet
                Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
                
                // Visa effekten genom att ändra storlek på diagramobjektet.
                chart.ChartObject.Width = actualSize[0];
                chart.ChartObject.Height = actualSize[1];
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


