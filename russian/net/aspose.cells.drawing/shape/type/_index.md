---
title: "Shape.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает тип автоматической фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/type/
---
## Shape.Type property

Получает тип автофигуры.

```csharp
public AutoShapeType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Получить и отобразить тип фигуры
            AutoShapeType autoShapeType = shape.Type;
            Console.WriteLine("Shape Type: " + autoShapeType);

            // Невозможно изменить тип фигуры, так как свойство Type только для чтения
            // Вместо этого создайте новую фигуру с другим типом
            Shape ovalShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Oval, 1, 1, 100, 150, 0, 0);
            Console.WriteLine("New Shape Type: " + ovalShape.Type);
        }
    }
}
```

### См. также

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


