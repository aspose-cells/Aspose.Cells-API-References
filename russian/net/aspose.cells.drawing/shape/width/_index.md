---
title: "Shape.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет ширину фигуры в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shape/width/
---
## Shape.Width property

Представляет ширину фигуры в пикселях.

```csharp
public int Width { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 50);

            // Установить начальную ширину и отобразить её
            shape.Width = 300;
            Console.WriteLine("Initial width: " + shape.Width);

            // Изменить ширину в зависимости от условия
            if (shape.Width == 300)
                shape.Width = 150;

            Console.WriteLine("Modified width: " + shape.Width);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


