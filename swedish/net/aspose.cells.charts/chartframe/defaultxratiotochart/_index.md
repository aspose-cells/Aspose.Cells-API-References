---
title: "ChartFrame.DefaultXRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame property. Representerar x‑koordinaten för standardpositionen i enheter av en bråkdel av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/defaultxratiotochart/
---
## ChartFrame.DefaultXRatioToChart property

Representerar x för standardpositionen i enheter av en bråkdel av diagramområdet.

```csharp
public double DefaultXRatioToChart { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta diagramrubrikens ram
            ChartFrame titleFrame = chart.Title;

            // Visa det aktuella värdet för DefaultXRatioToChart
            Console.WriteLine("Default X Ratio To Chart (Title): " + titleFrame.DefaultXRatioToChart);

            // Skapa en textruta i diagrammet
            Aspose.Cells.Drawing.TextBox textBox = chart.Shapes.AddTextBoxInChart(50, 50, 200, 100);
            
            // Hämta formegenskaperna för textrutan istället för att försöka komma åt ChartFrame direkt
            Console.WriteLine("Default X Ratio To Chart (TextBox): " + titleFrame.DefaultXRatioToChart);

            // Demonstrera hur dessa standardförhållanden påverkar positionering
            Console.WriteLine("Title X Position (Ratio): " + titleFrame.XRatioToChart);
            Console.WriteLine("TextBox X Position (Ratio): " + titleFrame.XRatioToChart);

            // Spara arbetsboken
            workbook.Save("ChartFrameDefaultXRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


