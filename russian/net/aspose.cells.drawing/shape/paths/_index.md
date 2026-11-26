---
title: "Shape.Paths"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает пути пользовательской геометрической фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/paths/
---
## Shape.Paths property

Получает пути пользовательской геометрической фигуры.

```csharp
public ShapePathCollection Paths { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPathsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пользовательскую фигуру (прямоугольник) с правильными параметрами
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 1, 1, 100, 150);

            // Проверить, имеет ли фигура пользовательские геометрические пути
            if (shape.Paths != null)
            {
                Console.WriteLine("Shape has custom geometry paths:");
                Console.WriteLine($"Number of paths: {shape.Paths.Count}");
                
                // Добавить новый путь к геометрии фигуры
                int newPathIndex = shape.Paths.Add();
                Console.WriteLine($"Added new path at index: {newPathIndex}");
            }
            else
            {
                Console.WriteLine("No custom geometry path.");
            }
        }
    }
}
```

### См. также

* class [ShapePathCollection](../../shapepathcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


