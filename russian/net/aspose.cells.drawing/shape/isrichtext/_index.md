---
title: "Shape.IsRichText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, является ли текст форматированным"
type: docs
url: /ru/net/aspose.cells.drawing/shape/isrichtext/
---
## Shape.IsRichText property

Определяет, является ли текст форматированным.

```csharp
public bool IsRichText { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsRichTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму с текстом
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is <b>rich</b> text";

            // Проверьте, является ли текст форматированным
            if (shape.IsRichText)
            {
                Console.WriteLine("The text is rich text.");
            }
            else
            {
                Console.WriteLine("The text is not rich text.");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


