---
title: "Shape.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет высоту фигуры в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shape/height/
---
## Shape.Height property

Представляет высоту фигуры в пикселях.

```csharp
public int Height { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Установить начальную высоту
            shape.Height = 150;
            Console.WriteLine("Initial height: " + shape.Height);

            // Изменить высоту условно
            if (shape.Height == 150)
            {
                shape.Height = 100;
                Console.WriteLine("Modified height: " + shape.Height);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


