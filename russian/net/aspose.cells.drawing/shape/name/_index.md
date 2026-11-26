---
title: "Shape.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задаёт имя фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/name/
---
## Shape.Name property

Получает и задает имя фигуры.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте фигуру и задайте её имя
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Name = "shape1";
            
            // Проверьте, что имя было установлено
            Console.WriteLine("Shape name: " + shape.Name);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


