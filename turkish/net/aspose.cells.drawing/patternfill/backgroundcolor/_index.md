---
title: "PatternFill.BackgroundColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PatternFill özelliği. Alanın arka plan Color'ını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/patternfill/backgroundcolor/
---
## PatternFill.BackgroundColor property

Arka plan Color'ını alır veya ayarlar [`Area`](../../area/).

```csharp
public Color BackgroundColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PatternFillPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
            
            shape.Fill.FillType = FillType.Pattern;
            shape.Fill.Pattern = FillPattern.SolidDiamond;
            shape.Fill.PatternFill.ForegroundColor = System.Drawing.Color.Red;
            shape.Fill.PatternFill.BackgroundColor = System.Drawing.Color.Green;

            workbook.Save("PatternFillBackgroundColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


