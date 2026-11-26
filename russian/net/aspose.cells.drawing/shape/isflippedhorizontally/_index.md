---
title: "Shape.IsFlippedHorizontally"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает, перевёрнута ли фигура по горизонтали"
type: docs
url: /ru/net/aspose.cells.drawing/shape/isflippedhorizontally/
---
## Shape.IsFlippedHorizontally property

Получает и задает, отражена ли фигура по горизонтали.

```csharp
public bool IsFlippedHorizontally { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFlippedHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Проверьте и переверните по горизонтали, если ещё не перевёрнута
            if (shape.IsFlippedHorizontally == false)
            {
                shape.IsFlippedHorizontally = true;
                Console.WriteLine("Shape was flipped horizontally");
            }
            else
            {
                Console.WriteLine("Shape was already flipped horizontally");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


