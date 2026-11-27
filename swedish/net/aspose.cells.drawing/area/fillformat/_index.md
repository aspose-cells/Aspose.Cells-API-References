---
title: "Area.FillFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Area-egenskap. Representerar ett FillFormat-objekt som innehåller fyllningsformateringsegenskaper för det angivna diagrammet eller formen"
type: docs
url: /sv/net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Representerar ett `FillFormat`-objekt som innehåller fyllningsformateringsegenskaper för det angivna diagrammet eller formen.

```csharp
public FillFormat FillFormat { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFillFormatDemo
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

            // Hämta den första seriens tredje punkt
            ChartPoint point = chart.NSeries[0].Points[2];
            
            // Ställ in fyllningsformatsegenskaper
            point.Area.FillFormat.Pattern = FillPattern.DashedHorizontal;
            point.Area.FillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.Horizontal, 2);

            // Spara arbetsboken
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Se även

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


