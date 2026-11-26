---
title: "Shape.Title"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает заголовок текущего объекта shape"
type: docs
url: /ru/net/aspose.cells.drawing/shape/title/
---
## Shape.Title property

Указывает заголовок (подпись) текущего объекта фигуры.

```csharp
public string Title { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Установите заголовок shape
            shape.Title = "title1";

            // Проверьте, что заголовок был установлен
            Console.WriteLine("Shape title: " + shape.Title);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


