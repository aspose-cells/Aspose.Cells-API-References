---
title: "MsoLineFormat.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoLineFormat. Возвращает или задаёт степень прозрачности указанного заполнения значением от 0.0 (непрозрачно) до 1.0 (полностью прозрачно)"
type: docs
url: /ru/net/aspose.cells.drawing/msolineformat/transparency/
---
## MsoLineFormat.Transparency property

Возвращает или задает степень прозрачности указанного заполнения в виде значения от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму дуги
            ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);

            // Установить свойства формата линии, включая прозрачность
            arc.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc.LineFormat.Transparency = 0.5; // 50% transparent
            arc.LineFormat.Weight = 3;
            arc.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Создать ещё одну дугу для сравнения
            ArcShape arc2 = worksheet.Shapes.AddArc(1, 2, 1, 2, 100, 100);
            arc2.LineFormat.ForeColor = System.Drawing.Color.Red;
            arc2.LineFormat.Transparency = 0.5; // Same transparency
            arc2.LineFormat.Weight = 3;
            arc2.LineFormat.DashStyle = MsoLineDashStyle.Solid;

            // Проверить свойство прозрачности
            if (Math.Abs(arc.LineFormat.Transparency - arc2.LineFormat.Transparency) < 0.001)
            {
                Console.WriteLine("Transparency properties match: " + arc.LineFormat.Transparency);
            }
            else
            {
                Console.WriteLine("Transparency properties do not match");
            }

            // Сохраните книгу
            workbook.Save("MsoLineFormatTransparencyDemo.xlsx");
        }
    }
}
```

### См. также

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


