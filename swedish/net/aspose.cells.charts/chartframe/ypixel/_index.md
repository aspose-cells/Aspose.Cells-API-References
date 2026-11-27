---
title: "ChartFrame.YPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i enheter av pixlar"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/ypixel/
---
## ChartFrame.YPixel property

Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i enheter av pixlar.

```csharp
public virtual int YPixel { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till diagramrubriken (som ärver från ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;

            // Visa aktuellt YPixel‑värde
            Console.WriteLine("Current YPixel value: " + chartFrame.YPixel);

            // Ändra YPixel‑positionen för diagramrubriken
            chartFrame.YPixel = 50;
            Console.WriteLine("New YPixel value: " + chartFrame.YPixel);

            // Spara arbetsboken
            workbook.Save("ChartFrameYPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


