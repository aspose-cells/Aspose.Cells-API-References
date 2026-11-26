---
title: "ShapeTextAlignment.TextShapeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeTextAlignment. Получает и задает тип преобразования текста"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/textshapetype/
---
## ShapeTextAlignment.TextShapeType property

Получает и задает тип трансформации текста.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);

            // Получить выравнивание текста формы
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Установите свойство TextShapeType
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;

            // Сохраните книгу
            workbook.Save("TextShapeTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


