---
title: "MsoLineFormat.BackColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormat. Получает и задаёт цвет фона линии границы"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Получает и задает цвет задней линии границы.

```csharp
public Color BackColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Установите свойства линии
            line.LineFormat.ForeColor = Color.Red;
            line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.0;

            // Сохраните книгу
            workbook.Save("LineFormatBackColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


