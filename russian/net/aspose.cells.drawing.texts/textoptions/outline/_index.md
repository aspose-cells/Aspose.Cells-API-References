---
title: "TextOptions.Outline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Представляет формат контура текста"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

Представляет формат контура текста.

```csharp
public LineFormat Outline { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyOutlineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму с текстом
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            shape.Text = "Sample Text";

            // Доступ к параметрам текста
            TextOptions textOptions = shape.TextOptions;

            // Настроить свойства контура
            LineFormat outline = textOptions.Outline;
            outline.Weight = 2.48; // Set outline weight
            outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
            outline.CompoundType = MsoLineStyle.Single; // Set compound type

            // Сохраните книгу
            workbook.Save("TextOutlineDemo.xlsx");
        }
    }
}
```

### См. также

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


