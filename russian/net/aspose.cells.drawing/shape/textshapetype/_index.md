---
title: "Shape.TextShapeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает предустановленный тип текстовой формы"
type: docs
url: /ru/net/aspose.cells.drawing/shape/textshapetype/
---
## Shape.TextShapeType property

Получает и задает предустановленный тип текстовой фигуры.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Проверьте и установите TextShapeType, если неизвестен
            if (shape.TextShapeType == AutoShapeType.Unknown)
            {
                shape.TextShapeType = AutoShapeType.Rectangle;
            }

            // Выведите TextShapeType формы
            Console.WriteLine("Shape TextShapeType: " + shape.TextShapeType);
        }
    }
}
```

### См. также

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


