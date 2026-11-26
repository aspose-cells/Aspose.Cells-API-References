---
title: "Column.ApplyStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Column. Применяет форматы для всей колонки"
type: docs
url: /ru/net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Применяет форматы ко всему столбцу.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Объект стиля, который будет применён. |
| флаг | StyleFlag | Флаги, указывающие применённые свойства форматирования. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установить многострочный текст в колонке 2
            sheet.Cells[0, 1].Value = "Line1\nLine2";
            sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
            sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";

            // Создать стиль с включённым переносом текста
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Применить стиль только к свойству переноса текста колонки 2
            sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


