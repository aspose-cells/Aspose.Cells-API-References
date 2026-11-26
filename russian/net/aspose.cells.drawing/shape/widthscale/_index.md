---
title: "Shape.WidthScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает масштаб ширины в процентах от исходной ширины изображения. Если форма не является изображением, свойство WidthScale возвращает только 100"
type: docs
url: /ru/net/aspose.cells.drawing/shape/widthscale/
---
## Shape.WidthScale property

Получает и задает масштаб ширины в процентах от исходной ширины изображения. Если фигура не является изображением, свойство WidthScale возвращает только 100;

```csharp
public int WidthScale { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Установите начальный масштаб ширины
            shape.WidthScale = 50;
            Console.WriteLine("Initial WidthScale: " + shape.WidthScale);

            // Измените масштаб ширины, если условие выполнено
            if (shape.WidthScale == 50)
            {
                shape.WidthScale = 75;
                Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
            }

            // Сохраните книгу
            workbook.Save("ShapeWidthScaleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


