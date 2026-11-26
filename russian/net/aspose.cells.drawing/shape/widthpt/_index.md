---
title: "Shape.WidthPt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет ширину фигуры в единицах пункта"
type: docs
url: /ru/net/aspose.cells.drawing/shape/widthpt/
---
## Shape.WidthPt property

Представляет ширину фигуры в пунктах.

```csharp
public double WidthPt { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthPtDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Установить и получить ширину в пунктах
            shape.WidthPt = 150;
            Console.WriteLine("Shape width in points: " + shape.WidthPt);

            // Изменить ширину, если условие выполнено
            if (shape.WidthPt == 150)
            {
                shape.WidthPt = 100;
                Console.WriteLine("Modified shape width in points: " + shape.WidthPt);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


