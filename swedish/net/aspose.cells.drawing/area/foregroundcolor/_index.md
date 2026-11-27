---
title: "Area.ForegroundColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Area-egenskap. Hämtar eller anger förgrundsfärgen"
type: docs
url: /sv/net/aspose.cells.drawing/area/foregroundcolor/
---
## Area.ForegroundColor property

Hämtar eller anger förgrundsfärgen.

```csharp
public Color ForegroundColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyForegroundColorDemo
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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange olika förgrundsfärger för varje serieområde
            chart.NSeries[0].Area.ForegroundColor = Color.FromArgb(79, 129, 189);
            chart.NSeries[1].Area.ForegroundColor = Color.FromArgb(192, 80, 77);

            // Spara arbetsboken
            workbook.Save("AreaForegroundColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


