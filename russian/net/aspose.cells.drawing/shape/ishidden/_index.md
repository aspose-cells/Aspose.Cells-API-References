---
title: "Shape.IsHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, видим ли объект"
type: docs
url: /ru/net/aspose.cells.drawing/shape/ishidden/
---
## Shape.IsHidden property

Указывает, видим ли объект.

```csharp
public bool IsHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Установить свойство IsHidden в false (видимый)
            shape.IsHidden = false;
            Console.WriteLine("Shape is visible: " + !shape.IsHidden);

            // Установить свойство IsHidden в true (скрытый)
            shape.IsHidden = true;
            Console.WriteLine("Shape is hidden: " + shape.IsHidden);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


