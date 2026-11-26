---
title: "ThreeDFormat.BottomBevelHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece la altura del bisel inferior o cuán profundo se aplica en la forma. En unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/bottombevelheight/
---
## ThreeDFormat.BottomBevelHeight property

Obtiene y establece la altura del bisel inferior, o cuán profundo se aplica en la forma. En unidades de puntos.

```csharp
public double BottomBevelHeight { get; set; }
```

### Ejemplos

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

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


