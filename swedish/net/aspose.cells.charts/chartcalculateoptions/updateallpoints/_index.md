---
title: "ChartCalculateOptions.UpdateAllPoints"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartCalculateOptions-egenskap. Anger om alla datapunkter ska uppdateras vid diagramberäkning. Standard False. När du vill hämta värdet för varje datapunkt i diagrammet, sätt den till true. Om denna parameter är satt till True kan nya datapunkter genereras när diagrammet beräknas. Detta kan göra Excel-filen större."
type: docs
url: /sv/net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Huruvida alla datapunkter ska uppdateras vid diagramberäkning. Standard: False. När du vill hämta värdet för varje datapunkt i diagrammet specifikt, sätt den till true. Om denna parameter är satt till True kan nya datapunkter genereras när diagrammet beräknas. Detta kan göra Excel-filen större.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(400);
            worksheet.Cells["C3"].PutValue(500);
            worksheet.Cells["C4"].PutValue(600);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Aktivera datamärkningar
            foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
            }

            // Beräkna diagram med UpdateAllPoints-alternativet
            chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });

            // Skriv ut några datalabelvärden för att demonstrera resultatet
            Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
            Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
        }
    }
}
```

### Se även

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


