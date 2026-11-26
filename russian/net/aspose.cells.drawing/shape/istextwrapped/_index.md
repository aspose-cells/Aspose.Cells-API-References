---
title: "Shape.IsTextWrapped"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает тип переноса текста формы, содержащей текст"
type: docs
url: /ru/net/aspose.cells.drawing/shape/istextwrapped/
---
## Shape.IsTextWrapped property

Получает и задает тип переноса текста в фигуре, содержащей текст.

```csharp
public bool IsTextWrapped { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму и задайте некоторый текст
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "This is a sample text that will demonstrate text wrapping functionality";

            // Продемонстрировать свойство IsTextWrapped
            Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
            
            // Переключите перенос текста
            shape.IsTextWrapped = !shape.IsTextWrapped;
            Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);

            // Сохраните книгу
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


