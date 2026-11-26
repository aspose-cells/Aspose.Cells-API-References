---
title: "LineFormat.BeginArrowheadStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LineFormat. Получает и задает тип начальной стрелки линии"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/beginarrowheadstyle/
---
## LineFormat.BeginArrowheadStyle property

Получает и задаёт тип начальной стрелки линии.

```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Установить стиль начальной стрелки
            line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Сохраните книгу
            workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


