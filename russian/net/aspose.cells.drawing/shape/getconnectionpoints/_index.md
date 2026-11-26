---
title: "Shape.GetConnectionPoints"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Получить точки соединения"
type: docs
url: /ru/net/aspose.cells.drawing/shape/getconnectionpoints/
---
## Shape.GetConnectionPoints method

Получить точки соединения

```csharp
public float[][] GetConnectionPoints()
```

### Возвращаемое значение

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetConnectionPointsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму на лист со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Получить точки соединения фигуры
            float[][] points = shape.GetConnectionPoints();

            // Вывести точки соединения
            Console.WriteLine("Connection Points:");
            for (int i = 0; i < points.Length; i++)
            {
                Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


