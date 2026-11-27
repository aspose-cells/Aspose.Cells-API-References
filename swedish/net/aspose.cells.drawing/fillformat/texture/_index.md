---
title: "FillFormat.Texture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskapen. Representerar texturtypen för den angivna fyllningen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/texture/
---
## FillFormat.Texture property

Representerar texturtypen för den angivna fyllningen.

```csharp
public TextureType Texture { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange textur för den första seriens tredje punkt
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Oak;

            // Spara arbetsboken
            workbook.Save("FillFormatTextureDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextureType](../../texturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


