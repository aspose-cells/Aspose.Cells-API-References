---
title: "LineFormat.CompoundType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LineFormat. Указывает составной тип линии"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/compoundtype/
---
## LineFormat.CompoundType property

Указывает составной тип линии.

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCompoundTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Получить формат линии
            LineFormat lineFmt = line.Line;

            // Установить составной тип
            lineFmt.CompoundType = MsoLineStyle.Single;

            // Сохраните книгу
            workbook.Save("LineFormatCompoundTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


