---
title: "ThreeDFormat.TopBevelType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta il tipo del bordo superiore o quanto in profondità nella forma viene applicato. In unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/topbeveltype/
---
## ThreeDFormat.TopBevelType property

Ottiene e imposta il tipo del bordo superiore, o quanto profondamente viene applicato nella forma. In unità di punti.

```csharp
public BevelType TopBevelType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            workbook.Save("ThreeDFormatTopBevelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


