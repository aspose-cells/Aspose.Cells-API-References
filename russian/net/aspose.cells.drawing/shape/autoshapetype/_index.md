---
title: "Shape.AutoShapeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает тип автофигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/autoshapetype/
---
## Shape.AutoShapeType property

Получает и задает тип автофигуры.

```csharp
public AutoShapeType AutoShapeType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAutoShapeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму в лист с правильными параметрами
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Проверьте и при необходимости измените AutoShapeType
            if (shape.AutoShapeType == AutoShapeType.Unknown)
            {
                shape.AutoShapeType = AutoShapeType.Rectangle;
            }

            // Измените тип фигуры, чтобы продемонстрировать свойство
            shape.AutoShapeType = AutoShapeType.Oval;

            // Сохраните книгу
            workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


