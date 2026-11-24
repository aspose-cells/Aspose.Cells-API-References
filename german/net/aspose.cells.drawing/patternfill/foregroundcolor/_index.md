---
title: "PatternFill.ForegroundColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PatternFill-Eigenschaft. Ruft die Vordergrundfarbe ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/patternfill/foregroundcolor/
---
## PatternFill.ForegroundColor property

Liest oder setzt die Vordergrundfarbe.

```csharp
public Color ForegroundColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PatternFillPropertyForegroundColorDemo
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

            workbook.Save("PatternFillForegroundColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


