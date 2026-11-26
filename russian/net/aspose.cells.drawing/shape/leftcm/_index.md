---
title: "Shape.LeftCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах"
type: docs
url: /ru/net/aspose.cells.drawing/shape/leftcm/
---
## Shape.LeftCM property

Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах.

```csharp
public double LeftCM { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftCMDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установить и получить свойство LeftCM
            shape.LeftCM = 3.0;
            Console.WriteLine("Shape left position (cm): " + shape.LeftCM);

            // Изменить левое положение, если оно равно 3 см
            if (shape.LeftCM == 3.0)
            {
                shape.LeftCM = 1.0;
                Console.WriteLine("Adjusted shape left position (cm): " + shape.LeftCM);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


