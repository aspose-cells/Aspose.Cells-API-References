---
title: "SolidFill.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SolidFill. Получает или задает Color"
type: docs
url: /ru/net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Получает или задает цвет.

```csharp
public Color Color { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить форму в лист с правильными параметрами
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Установить свойства формы с цветом
            Color fillColor = Color.LightBlue;
            Color textColor = Color.DarkBlue;
            string text = "Solid Fill Demo";

            // Продемонстрировать использование свойства Color
            shape.Fill.SolidFill.Color = fillColor;
            shape.LineFormat.ForeColor = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;

            // Сохраните книгу
            workbook.Save("SolidFillPropertyColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


