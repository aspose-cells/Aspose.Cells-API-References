---
title: "Перечисление LineCapType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.LineCapType. Представляет концы линии"
type: docs
url: /ru/net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Представляет окончания линии.

```csharp
public enum LineCapType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Square | `0` | Квадрат выступает на половину ширины линии. |
| Round | `1` | Закруглённые концы. |
| Flat | `2` | Линия заканчивается в конечной точке. |
| None | `3` | Нет крышки |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
            
            LineFormat lineFmt = shape.Line;
            lineFmt.CapType = LineCapType.Flat;
            lineFmt.Weight = 2.0;
            lineFmt.DashStyle = MsoLineDashStyle.Solid;
            
            workbook.Save("LineCapTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


