---
title: "Перечисление MsoArrowheadStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.MsoArrowheadStyle. Перечисляет тип окончания линии границы фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Перечисляет тип конца линии границы фигуры.

```csharp
public enum MsoArrowheadStyle
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без типа окончания линии. |
| Arrow | `1` | Тип окончания линии со стрелкой. |
| ArrowStealth | `2` | Тип окончания линии со скрытой стрелкой. |
| ArrowDiamond | `3` | Тип окончания линии со стрелкой-ромбом. |
| ArrowOval | `4` | Тип окончания линии со стрелкой-овалом. |
| ArrowOpen | `5` | Тип окончания линии со открытой стрелкой. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassMsoArrowheadStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте линейную фигуру
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);

            // Установите свойства линии
            MsoLineFormat lineFormat = lineShape.LineFormat;
            lineFormat.ForeColor = System.Drawing.Color.Black;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 0.75;

            // Установите стили наконечников стрелок
            lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
            lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;

            // Сохраните книгу
            workbook.Save("MsoArrowheadStyleDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


