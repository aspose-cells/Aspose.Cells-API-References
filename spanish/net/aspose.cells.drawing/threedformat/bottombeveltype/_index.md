---
title: "ThreeDFormat.BottomBevelType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece el tipo del bisel inferior o qué tan profundo se aplica en la forma. En unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/bottombeveltype/
---
## ThreeDFormat.BottomBevelType property

Obtiene y establece el tipo del bisel inferior, o cuán profundo se aplica en la forma. En unidades de puntos.

```csharp
public BevelType BottomBevelType { get; set; }
```

### Ejemplos

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

### Ver también

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


