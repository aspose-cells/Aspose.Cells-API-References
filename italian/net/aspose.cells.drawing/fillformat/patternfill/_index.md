---
title: "FillFormat.PatternFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene l'oggetto PatternFill"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/patternfill/
---
## FillFormat.PatternFill property

Ottiene l'oggetto `PatternFill`.

```csharp
public PatternFill PatternFill { get; }
```

### Esempi

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

### Vedi anche

* class [PatternFill](../../patternfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


