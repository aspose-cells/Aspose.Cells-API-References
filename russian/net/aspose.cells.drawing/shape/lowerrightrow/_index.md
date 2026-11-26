---
title: "Shape.LowerRightRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет индекс строки нижнего правого угла"
type: docs
url: /ru/net/aspose.cells.drawing/shape/lowerrightrow/
---
## Shape.LowerRightRow property

Представляет индекс строки нижнего правого угла.

```csharp
public int LowerRightRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установите и продемонстрируйте свойство LowerRightRow
            Console.WriteLine("Original LowerRightRow: " + shape.LowerRightRow);
            shape.LowerRightRow = 3;
            Console.WriteLine("Modified LowerRightRow: " + shape.LowerRightRow);

            // Условное изменение в соответствии с тестовым случаем
            if (shape.LowerRightRow == 3)
            {
                shape.LowerRightRow = 1;
                Console.WriteLine("Final LowerRightRow after condition: " + shape.LowerRightRow);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


