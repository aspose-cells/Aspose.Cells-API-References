---
title: "Shape.IsPrintable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, печатается ли объект. Если False, эта фигура не будет печататься при печати"
type: docs
url: /ru/net/aspose.cells.drawing/shape/isprintable/
---
## Shape.IsPrintable property

Указывает, печатается ли объект. Если False, эта фигура не будет печататься.

```csharp
public bool IsPrintable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsPrintableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Продемонстрировать свойство IsPrintable
            Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);

            // Переключить свойство IsPrintable
            shape.IsPrintable = !shape.IsPrintable;
            Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);

            // Установить IsPrintable в false явно
            shape.IsPrintable = false;
            Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


