---
title: "FillFormat.PatternFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تحصل على كائن PatternFill"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/patternfill/
---
## FillFormat.PatternFill property

يحصل على كائن `PatternFill`.

```csharp
public PatternFill PatternFill { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPatternFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 100, 50, 50);
            
            shape.Fill.FillType = FillType.Pattern;
            shape.Fill.Pattern = FillPattern.HorizontalBrick;
            shape.Fill.PatternFill.ForegroundColor = System.Drawing.Color.Blue;
            shape.Fill.PatternFill.BackgroundColor = System.Drawing.Color.Yellow;

            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PatternFill](../../patternfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


