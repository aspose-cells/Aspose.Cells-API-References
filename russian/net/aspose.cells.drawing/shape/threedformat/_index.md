---
title: "Shape.ThreeDFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает 3D-формат фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/threedformat/
---
## Shape.ThreeDFormat property

Получает и задает 3D-формат фигуры.

```csharp
public ThreeDFormat ThreeDFormat { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyThreeDFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Получать и изменять свойства 3D-формата
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.LightAngle = 45;
            threeDFormat.ContourWidth = 2;
            threeDFormat.ContourColor.Color = System.Drawing.Color.Red;

            // Сохраните книгу
            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../../threedformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


