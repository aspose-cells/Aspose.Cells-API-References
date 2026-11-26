---
title: "Cells.ApplyRowStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Применяет форматы ко всей строке"
type: docs
url: /ru/net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

Применяет форматы к целой строке.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| стиль | Стиль | Объект стиля, который будет применён. |
| флаг | StyleFlag | Флаги, указывающие применённые свойства форматирования. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать стиль с границами
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Создайте флаг стиля для границ
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Примените стиль к первой строке
            cells.ApplyRowStyle(0, style, styleFlag);

            // Сохраните книгу
            workbook.Save("ApplyRowStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


