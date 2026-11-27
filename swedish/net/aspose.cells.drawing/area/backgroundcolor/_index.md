---
title: "Area.BackgroundColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Area-egenskap. Hämtar eller anger bakgrundsfärgen för Area"
type: docs
url: /sv/net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Hämtar eller anger bakgrundsfärgen för [`Area`](../).

```csharp
public Color BackgroundColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Ange bakgrundsfärg för kategoriaxelområdet
            chart.CategoryAxis.Area.BackgroundColor = System.Drawing.Color.Red;

            // Visa bakgrundsfärgen
            Console.WriteLine("Category Axis Background Color: " + chart.CategoryAxis.Area.BackgroundColor);

            // Spara arbetsboken
            workbook.Save("AreaPropertyBackgroundColorDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


