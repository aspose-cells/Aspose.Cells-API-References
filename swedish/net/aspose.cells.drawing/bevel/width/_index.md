---
title: "Bevel.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Bevel egenskap. Hämtar och anger bredden på avfasningen eller hur långt in i formen den tillämpas. I enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Hämtar och anger bredden på avfasningen, eller hur djupt in i formen den tillämpas. I enheten punkter.

```csharp
public double Width { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyWidthDemo
    {
        public static void Run()
        {
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

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta första serien och ange 3D-format
            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;
            
            // Konfigurera avfasningsegenskaper med bredddemonstration
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 12; // Demonstrating Width property
            topBevel.Height = 6;

            // Spara arbetsboken
            workbook.Save("BevelWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


