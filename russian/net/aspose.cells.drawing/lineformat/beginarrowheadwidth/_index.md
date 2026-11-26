---
title: "LineFormat.BeginArrowheadWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LineFormat. Получает и задает тип ширины начальной стрелки линии"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/beginarrowheadwidth/
---
## LineFormat.BeginArrowheadWidth property

Получает и задаёт тип ширины начальной стрелки линии.

```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Установить свойства формата линии
            LineFormat lineFmt = line.Line;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Сохраните книгу
            workbook.Save("LineFormatDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


