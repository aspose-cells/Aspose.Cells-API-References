---
title: "LineFormat.EndArrowheadStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LineFormat. Получает и задает тип конечной стрелки линии"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/endarrowheadstyle/
---
## LineFormat.EndArrowheadStyle property

Получает и задаёт тип конечной стрелки линии.

```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Получить формат линии
            LineFormat lineFmt = line.Line;

            // Установить стиль конечной стрелки
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Сохраните книгу
            workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


