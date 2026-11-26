---
title: "LineFormat.JoinType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LineFormat. Указывает тип соединения линии"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

Указывает тип соединения линии.

```csharp
public LineJoinType JoinType { get; set; }
```

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyJoinTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму линии
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Установить тип соединения линии в Round
            line.Line.JoinType = LineJoinType.Round;

            // Сохраните книгу
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


