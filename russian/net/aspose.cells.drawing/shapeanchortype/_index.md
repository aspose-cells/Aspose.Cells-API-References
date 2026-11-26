---
title: "Перечисление ShapeAnchorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.ShapeAnchorType перечисление. Представляет тип привязки"
type: docs
url: /ru/net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

Представляет тип привязки.

```csharp
public enum ShapeAnchorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| TwoCellAnchor | `0` | Представляет заполнитель привязки в две ячейки |
| OneCellAnchor | `1` | Представляет заполнитель привязки в одну ячейку |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму группы
            Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
            box.Text = "Sample Group Box";
            
            // Продемонстрировать использование ShapeAnchorType
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 2;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 8;
            box.LowerRightColumn = 4;

            // Сохраните книгу
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


