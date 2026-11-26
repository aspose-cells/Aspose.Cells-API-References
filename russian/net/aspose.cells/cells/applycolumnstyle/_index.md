---
title: "Cells.ApplyColumnStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Применяет форматы ко всей колонке"
type: docs
url: /ru/net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Применяет форматы ко всему столбцу.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |
| стиль | Стиль | Объект стиля, который будет применён. |
| флаг | StyleFlag | Флаги, указывающие применённые свойства форматирования. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Создать стиль с границами
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Создать флаг стиля, чтобы применять только границы
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            // Применить стиль к столбцу 1 (индекс 0)
            cells.ApplyColumnStyle(0, style, sflag);

            // Сохраните книгу
            workbook.Save("ApplyColumnStyleOutput.xlsx");
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


