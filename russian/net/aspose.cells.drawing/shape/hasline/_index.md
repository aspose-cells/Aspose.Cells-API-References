---
title: "Shape.HasLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает видимость границы линии фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/hasline/
---
## Shape.HasLine property

Получает и задает видимость линии границы фигуры.

```csharp
public bool HasLine { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHasLineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Продемонстрировать свойство HasLine
            Console.WriteLine("Shape initially has line: " + shape.HasLine);
            
            // Удалить линию
            shape.HasLine = false;
            Console.WriteLine("After setting HasLine to false: " + shape.HasLine);
            
            // Добавить линию обратно
            shape.HasLine = true;
            Console.WriteLine("After setting HasLine to true: " + shape.HasLine);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


