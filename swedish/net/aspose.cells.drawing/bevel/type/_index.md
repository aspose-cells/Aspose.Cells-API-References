---
title: "Bevel.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Bevel egenskap. Hämtar och anger den förinställda avfasningstypen"
type: docs
url: /sv/net/aspose.cells.drawing/bevel/type/
---
## Bevel.Type property

Hämtar och anger den förinställda avfasningstypen.

```csharp
public BevelPresetType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyTypeDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagramdata
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta den första serien
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Ställ in seriefärg
            series.Area.ForegroundColor = Color.Blue;

            // Konfigurera 3D-format och avfasningsegenskaper
            Format3D format3D = series.ShapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            // Demonstrera användning av Type-egenskapen
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 5;
            topBevel.Height = 2;

            // Spara arbetsboken
            workbook.Save("BevelPropertyTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [BevelPresetType](../../bevelpresettype/)
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


