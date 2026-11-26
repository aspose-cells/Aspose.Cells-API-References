---
title: "ShapeTextAlignment.RotationAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeTextAlignment. Получает и задает вращение фигуры"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/rotationangle/
---
## ShapeTextAlignment.RotationAngle property

Получает и задает вращение фигуры.

```csharp
public double RotationAngle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 200, 300, 400);
            
            // Установить текст фигуры
            shape.Text = "Rotated Text";
            
            // Получить выравнивание текста и установить угол вращения
            shape.TextBody.TextAlignment.RotationAngle = 90;

            // Сохраните книгу
            workbook.Save("ShapeTextRotationDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


