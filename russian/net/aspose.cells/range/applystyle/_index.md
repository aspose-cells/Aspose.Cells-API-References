---
title: "Range.ApplyStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Применяет форматы ко всему диапазону"
type: docs
url: /ru/net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Применяет форматы ко всему диапазону.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Объект стиля, который будет применён. |
| флаг | StyleFlag | Флаги, указывающие применённые свойства форматирования. |

### Примечания

Каждая ячейка в этом диапазоне будет содержать объект [`Style`](../../style/). Поэтому этот метод потребляет много памяти. Пожалуйста, используйте его осторожно.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;

            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("Sample text for style demonstration");

            Aspose.Cells.Range range = cells.CreateRange(0, 0, 1, 3);

            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            styleFlag.VerticalAlignment = true;
            styleFlag.WrapText = true;

            range.ApplyStyle(style, styleFlag);

            workbook.Save("ApplyStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


