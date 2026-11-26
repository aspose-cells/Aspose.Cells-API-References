---
title: "MsoLineFormat.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormat. Возвращает объект Style, представляющий стиль указанного диапазона"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

Возвращает объект Style, который представляет стиль указанного диапазона.

```csharp
public MsoLineStyle Style { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);

            // Получить формат линии
            MsoLineFormat lineFormat = line.LineFormat;

            // Установить свойства стиля линии
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.BackColor = System.Drawing.Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // Создать ещё одну линию для сравнения
            Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
            MsoLineFormat lineFormat2 = line2.LineFormat;

            // Скопировать стиль с первой линии на вторую линию
            lineFormat2.Style = lineFormat.Style;
            lineFormat2.ForeColor = lineFormat.ForeColor;
            lineFormat2.BackColor = lineFormat.BackColor;
            lineFormat2.DashStyle = lineFormat.DashStyle;
            lineFormat2.Transparency = lineFormat.Transparency;
            lineFormat2.Weight = lineFormat.Weight;

            // Сохраните книгу
            workbook.Save("MsoLineFormatStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


