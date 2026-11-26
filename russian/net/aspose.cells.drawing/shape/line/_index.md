---
title: "Shape.Line"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает стиль линии"
type: docs
url: /ru/net/aspose.cells.drawing/shape/line/
---
## Shape.Line property

Получает стиль линии

```csharp
public LineFormat Line { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму линии (возвращает LineShape напрямую)
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);

            // Получить доступ и изменить свойства линии
            LineFormat lineFormat = lineShape.Line;
            lineFormat.CompoundType = MsoLineStyle.ThickThin;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 3.0;
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Сохраните книгу
            workbook.Save("LineShapeDemo.xlsx");
        }
    }
}
```

### См. также

* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


