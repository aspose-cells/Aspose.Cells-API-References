---
title: "LineFormat.CapType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LineFormat. Указывает конечные заглушки"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/captype/
---
## LineFormat.CapType property

Указывает конечные заглушки.

```csharp
public LineCapType CapType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Установить свойства формата линии
            LineFormat lineFmt = line.Line;
            lineFmt.CapType = LineCapType.Flat;

            // Сохраните книгу
            workbook.Save("LineFormatCapTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


