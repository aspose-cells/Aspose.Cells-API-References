---
title: "Shape.Spt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает необязательный номер, который приложение может использовать для связывания конкретной фигуры с определённым типом фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/spt/
---
## Shape.Spt property

Указывает необязательное число, которое приложение может использовать для связывания конкретной фигуры с определённым типом фигуры.

```csharp
public int Spt { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySptDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);

            // Получите и отобразите свойство Spt
            int spt = shape.Spt;
            Console.WriteLine("Shape Spt value: " + spt);

            // Создайте новую овальную фигуру, чтобы продемонстрировать различное значение Spt
            Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
            Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


