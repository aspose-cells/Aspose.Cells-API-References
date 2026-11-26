---
title: "Shape.TopToCorner"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает вертикальное смещение формы от верхней границы листа в единицах пикселей"
type: docs
url: /ru/net/aspose.cells.drawing/shape/toptocorner/
---
## Shape.TopToCorner property

Получает и задает вертикальное смещение фигуры от верхнего края листа в пикселях.

```csharp
public int TopToCorner { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopToCornerDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Задайте и отобразите свойство TopToCorner
            shape.TopToCorner = 50;
            Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);

            // Измените свойство TopToCorner
            if (shape.TopToCorner == 50)
            {
                shape.TopToCorner = 20;
                Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


