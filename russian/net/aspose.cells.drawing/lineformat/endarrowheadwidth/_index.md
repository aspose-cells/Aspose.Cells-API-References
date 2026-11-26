---
title: "LineFormat.EndArrowheadWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LineFormat. Получает и задает тип ширины конечной стрелки линии"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/endarrowheadwidth/
---
## LineFormat.EndArrowheadWidth property

Получает и задаёт тип ширины конечной стрелки линии.

```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);

            // Получить формат линии
            LineFormat lineFmt = line.Line;

            // Установить ширину конечной стрелки
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Сохраните книгу
            workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


