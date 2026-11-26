---
title: "Shape.UpperLeftRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет индекс верхней строки"
type: docs
url: /ru/net/aspose.cells.drawing/shape/upperleftrow/
---
## Shape.UpperLeftRow property

Представляет индекс верхней строки.

```csharp
public int UpperLeftRow { get; set; }
```

### Примечания

Если фигура находится в фигуре или в группе, UpperLeftRow будет игнорироваться.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Установить и продемонстрировать свойство UpperLeftRow
            shape.UpperLeftRow = 3;
            Console.WriteLine("Shape's initial topRow: " + shape.UpperLeftRow);

            // Изменить UpperLeftRow в зависимости от условия
            if (shape.UpperLeftRow == 3)
                shape.UpperLeftRow = 1;

            Console.WriteLine("Shape's modified topRow: " + shape.UpperLeftRow);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


