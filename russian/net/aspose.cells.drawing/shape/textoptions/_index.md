---
title: "Shape.TextOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет параметры текста фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/textoptions/
---
## Shape.TextOptions property

Представляет параметры текста фигуры.

```csharp
public TextOptions TextOptions { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Установите текст для формы
            shape.Text = "Sample Text";

            // Получите доступ и измените TextOptions
            TextOptions opt = shape.TextOptions;
            opt.Color = Color.Blue;
            opt.Size = 8;

            // Сохраните книгу
            workbook.Save("ShapeTextOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


