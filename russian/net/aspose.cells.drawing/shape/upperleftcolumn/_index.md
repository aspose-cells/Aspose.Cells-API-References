---
title: "Shape.UpperLeftColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет индекс столбца верхнего левого угла"
type: docs
url: /ru/net/aspose.cells.drawing/shape/upperleftcolumn/
---
## Shape.UpperLeftColumn property

Представляет индекс столбца верхнего левого угла.

```csharp
public int UpperLeftColumn { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму на лист со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 100);

            // Установите и продемонстрируйте свойство UpperLeftColumn
            shape.UpperLeftColumn = 3;
            Console.WriteLine("Shape's initial leftColumn: " + shape.UpperLeftColumn);

            // Изменить UpperLeftColumn
            if (shape.UpperLeftColumn == 3)
            {
                shape.UpperLeftColumn = 1;
                Console.WriteLine("Shape's modified leftColumn: " + shape.UpperLeftColumn);
            }

            // Сохраните книгу
            workbook.Save("ShapeUpperLeftColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


