---
title: "Shape.Right"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет ширину горизонтального смещения фигуры от её нижнего правого столбца в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shape/right/
---
## Shape.Right property

Представляет ширину горизонтального смещения фигуры от её нижнего правого столбца, в пикселях.

```csharp
public int Right { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Установите и получите свойство Right
            shape.Right = 200;
            Console.WriteLine("Shape Right position: " + shape.Right);

            // Измените свойство Right условно
            if (shape.Right == 200)
                shape.Right = 150;

            Console.WriteLine("Modified Shape Right position: " + shape.Right);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


