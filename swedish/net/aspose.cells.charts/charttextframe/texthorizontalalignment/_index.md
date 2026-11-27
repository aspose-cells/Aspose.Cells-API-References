---
title: "ChartTextFrame.TextHorizontalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Hämtar och anger den horisontella justeringen av text"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/texthorizontalalignment/
---
## ChartTextFrame.TextHorizontalAlignment property

Hämtar och anger horisontell justering av texten.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextHorizontalAlignmentDemo
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

            // Lägg till ett diagram och ange dess dataintervall
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta diagramtiteln och ange egenskaper
            Title title = chart.Title;
            title.Text = "Sample Chart Title";
            
            // Demonstrera TextHorizontalAlignment-egenskapen
            title.TextHorizontalAlignment = TextAlignmentType.Center;
            Console.WriteLine("Title horizontal alignment set to: " + title.TextHorizontalAlignment);

            // Spara arbetsboken
            workbook.Save("ChartTextHorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


