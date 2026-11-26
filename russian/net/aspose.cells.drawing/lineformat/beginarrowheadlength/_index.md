---
title: "LineFormat.BeginArrowheadLength"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LineFormat. Получает и задает тип длины начальной стрелки линии"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/beginarrowheadlength/
---
## LineFormat.BeginArrowheadLength property

Получает и задаёт тип длины начальной стрелки линии.

```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
            LineShape line = (LineShape)lineShape;

            // Установить длину начальной стрелки
            line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;

            // Сохраните книгу
            workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


