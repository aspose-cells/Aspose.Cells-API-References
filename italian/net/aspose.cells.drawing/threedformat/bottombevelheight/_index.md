---
title: "ThreeDFormat.BottomBevelHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta l'altezza dello smusso inferiore o quanto profondamente viene applicato nella forma. In unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/bottombevelheight/
---
## ThreeDFormat.BottomBevelHeight property

Ottiene e imposta l'altezza del bordo inferiore, o quanto è applicato alla forma. In unità di punti.

```csharp
public double BottomBevelHeight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyBottomBevelHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.BottomBevelType = BevelType.Circle;
            threeDFormat.BottomBevelWidth = 8;
            threeDFormat.BottomBevelHeight = 12;

            workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


