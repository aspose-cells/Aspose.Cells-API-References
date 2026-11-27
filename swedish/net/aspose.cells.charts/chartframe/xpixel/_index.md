---
title: "ChartFrame.XPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av Pixel"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/xpixel/
---
## ChartFrame.XPixel property

Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av pixel.

```csharp
public virtual int XPixel { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXPixelDemo
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
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Åtkomst till diagramrubriken (som ärver från ChartFrame)
            chart.Title.Text = "Sample Chart";
            
            // Visa aktuell XPixel‑position för titeln
            Console.WriteLine("Current Title XPixel position: " + chart.Title.XPixel);
            
            // Flytta titeln horisontellt genom att ändra XPixel
            chart.Title.XPixel = 200;
            
            // Visa den nya XPixel‑positionen
            Console.WriteLine("New Title XPixel position: " + chart.Title.XPixel);
            
            // Spara arbetsboken
            workbook.Save("ChartFrameXPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


