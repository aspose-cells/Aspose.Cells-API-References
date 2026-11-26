---
title: "ThreeDFormat.TopBevelType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает тип верхнего фаски или глубину её применения к фигуре. В единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/topbeveltype/
---
## ThreeDFormat.TopBevelType property

Получает и задает тип верхней фаски, или насколько глубоко она применяется к фигуре. В единицах точек.

```csharp
public BevelType TopBevelType { get; set; }
```

### Примеры

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

### См. также

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


