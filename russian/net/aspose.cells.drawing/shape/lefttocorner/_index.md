---
title: "Shape.LeftToCorner"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает горизонтальное смещение фигуры от левого края листа"
type: docs
url: /ru/net/aspose.cells.drawing/shape/lefttocorner/
---
## Shape.LeftToCorner property

Получает и задает горизонтальное смещение фигуры от левого края листа.

```csharp
public int LeftToCorner { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftToCornerDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Установите и продемонстрируйте свойство LeftToCorner
            shape.LeftToCorner = 50;
            Console.WriteLine("Shape LeftToCorner value: " + shape.LeftToCorner);

            // Измените LeftToCorner, если он равен определённому значению
            if (shape.LeftToCorner == 50)
            {
                shape.LeftToCorner = 30;
                Console.WriteLine("Modified LeftToCorner value: " + shape.LeftToCorner);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


