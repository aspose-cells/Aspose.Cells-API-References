---
title: "Row.ApplyStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Row. Применяет форматы для всей строки"
type: docs
url: /ru/net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Применяет форматы к целой строке.

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
    public class RowMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установить HTML‑содержимое в первой ячейке
            sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";

            // Получить первую строку и её стиль
            Row row = sheet.Cells.Rows[0];
            Style style = row.GetStyle();
            
            // Изменить свойства стиля
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // Применить стиль с определёнными флагами (будет применено только перенос текста)
            row.ApplyStyle(style, new StyleFlag { WrapText = true });

            // Автоподгонка для демонстрации
            sheet.AutoFitRows();
            sheet.AutoFitColumns();

            // Сохраните книгу
            workbook.Save("RowApplyStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


