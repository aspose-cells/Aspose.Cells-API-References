---
title: "ChartFrame.HeightRatioToChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar eller anger höjden på ramen i enheter av förhållandet till diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/heightratiotochart/
---
## ChartFrame.HeightRatioToChart property

Hämtar eller anger höjden för ramen i enheter av förhållandet till diagramområdet.

```csharp
public virtual double HeightRatioToChart { get; set; }
```

### Anmärkningar

Detta är ett bråktal, dess giltiga intervall är mellan 0-1. Hur konverterar man enheter av förhållandet till pixlar? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till diagramrubriken (som ärver från ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame titleFrame = chart.Title;

            // Visa aktuellt HeightRatioToChart‑värde
            Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);

            // Ställ in ett nytt höjdförhållande (0.1 = 10% av diagramhöjden)
            titleFrame.HeightRatioToChart = 0.1;

            // Visa effekten genom att jämföra före/efter
            Console.WriteLine("Title height reduced to 10% of chart height");

            // Spara resultatet
            workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


