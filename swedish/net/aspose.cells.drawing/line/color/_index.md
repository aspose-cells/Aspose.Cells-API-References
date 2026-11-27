---
title: "Line.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Line-egenskap. Representerar färgen på linjen"
type: docs
url: /sv/net/aspose.cells.drawing/line/color/
---
## Line.Color property

Representerar färgen på linjen.

```csharp
public Color Color { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in färger för axellinjer
            chart.CategoryAxis.AxisLine.Color = Color.BlueViolet;
            chart.ValueAxis.AxisLine.Color = Color.BlueViolet;
            
            // Ställ in färg på axelrubrikens teckensnitt
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.Font.Color = Color.BlueViolet;

            // Spara arbetsboken
            workbook.Save("LinePropertyColorDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


