---
title: "ThreeDFormat.BottomBevelType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает тип нижнего фаски или насколько глубоко она применяется к фигуре. В единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/bottombeveltype/
---
## ThreeDFormat.BottomBevelType property

Получает и задает тип нижнего скоса, или насколько глубоко он применяется к фигуре. В единицах точек.

```csharp
public BevelType BottomBevelType { get; set; }
```

### Примеры

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

### См. также

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


