---
title: "ThreeDFormat.BottomBevelType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta il tipo di smusso inferiore o quanto in profondità viene applicato alla forma. In unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/bottombeveltype/
---
## ThreeDFormat.BottomBevelType property

Ottiene e imposta il tipo del bordo inferiore, o quanto è applicato alla forma. In unità di punti.

```csharp
public BevelType BottomBevelType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyBottomBevelTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 8;
            threeDFormat.BottomBevelHeight = 8;

            workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


