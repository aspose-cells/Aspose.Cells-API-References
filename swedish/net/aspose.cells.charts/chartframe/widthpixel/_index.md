---
title: "ChartFrame.WidthPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar eller anger bredden på ramen i enheter av Pixel"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/widthpixel/
---
## ChartFrame.WidthPixel property

Hämtar eller anger bredden på ramen i enheter av pixel.

```csharp
public virtual int WidthPixel { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthPixelDemo
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
            
            // Visa aktuellt WidthPixel‑värde för diagramrubriken
            Console.WriteLine("Current Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Ställ in en ny bredd för diagramrubriken i pixlar
            chart.Title.WidthPixel = 300;
            
            // Visa det nya WidthPixel‑värdet
            Console.WriteLine("New Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Spara arbetsboken
            workbook.Save("ChartFrameWidthPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


