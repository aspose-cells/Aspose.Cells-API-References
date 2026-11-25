---
title: "ThreeDFormat.BottomBevelWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta la larghezza del contorno inferiore o quanto profondamente viene applicata alla forma. In unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/bottombevelwidth/
---
## ThreeDFormat.BottomBevelWidth property

Ottiene e imposta la larghezza del bordo inferiore, o quanto è applicato alla forma. In unità di punti.

```csharp
public double BottomBevelWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyBottomBevelWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.BottomBevelType = BevelType.ArtDeco;
            threeDFormat.BottomBevelWidth = 15;
            threeDFormat.BottomBevelHeight = 8;

            workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


