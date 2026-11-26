---
title: "Shape.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет шрифт фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/font/
---
## Shape.Font property

Представляет шрифт фигуры.

```csharp
public Font Font { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Получить доступ и изменить свойства шрифта фигуры
            Aspose.Cells.Font font = shape.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;

            // Сохраните книгу
            workbook.Save("ShapeFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


