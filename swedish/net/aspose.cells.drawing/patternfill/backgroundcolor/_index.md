---
title: "PatternFill.BackgroundColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PatternFill-egenskap. Hämtar eller anger bakgrundsfärgen för Area"
type: docs
url: /sv/net/aspose.cells.drawing/patternfill/backgroundcolor/
---
## PatternFill.BackgroundColor property

Hämtar eller anger bakgrundsfärgen för [`Area`](../../area/).

```csharp
public Color BackgroundColor { get; set; }
```

### Exempel

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

### Se även

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


