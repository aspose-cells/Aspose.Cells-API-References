---
title: "ShapeTextAlignment.RotateTextWithShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeTextAlignment. Указывает, вращать ли текст вместе с формой"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/
---
## ShapeTextAlignment.RotateTextWithShape property

Указывает, вращается ли текст вместе с формой.

```csharp
public bool RotateTextWithShape { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля с правильными параметрами
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Получите свойства выравнивания текста
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            
            // Установите свойство RotateTextWithShape
            textAlignment.RotateTextWithShape = true;

            // Поверните форму, чтобы продемонстрировать эффект
            shape.RotationAngle = 45;

            // Сохраните книгу
            workbook.Save("RotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


