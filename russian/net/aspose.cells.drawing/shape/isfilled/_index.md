---
title: "Shape.IsFilled"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, видим ли формат заливки"
type: docs
url: /ru/net/aspose.cells.drawing/shape/isfilled/
---
## Shape.IsFilled property

Указывает, видим ли формат заливки.

```csharp
public bool IsFilled { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFilledDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Проверьте и измените свойство IsFilled
            if (shape.IsFilled == false)
            {
                shape.IsFilled = true;
                shape.FillFormat.ForeColor = System.Drawing.Color.Red;
            }

            // Сохраните книгу
            workbook.Save("ShapeIsFilledDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


