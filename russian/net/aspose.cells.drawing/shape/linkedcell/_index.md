---
title: "Shape.LinkedCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает или задает диапазон листа, связанный со значением controls"
type: docs
url: /ru/net/aspose.cells.drawing/shape/linkedcell/
---
## Shape.LinkedCell property

Получает или задает диапазон листа, связанный со значением элемента управления.

```csharp
public string LinkedCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Установите свойство LinkedCell в B6
            shape.LinkedCell = "$B$6";

            // Измените LinkedCell на A1, если он был B6
            if (shape.LinkedCell.Equals("$B$6"))
            {
                shape.LinkedCell = "A1";
            }

            // Выведите текущее значение LinkedCell
            Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


