---
title: "ChartFrame.HeightPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar eller anger höjden på ramen i enheter av pixlar"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

Hämtar eller anger höjden för ramen i enheter av pixlar.

```csharp
public virtual int HeightPixel { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            
            // Åtkomst till diagramtiteln (som är en ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // Visa aktuell höjd i pixlar
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // Ange en ny höjd för titeln
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // Åtkomst till förklaringen (en annan ChartFrame)
            ChartFrame legend = chart.Legend;
            
            // Visa och ändra legendens höjd
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // Spara arbetsboken
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


