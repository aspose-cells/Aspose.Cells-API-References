---
title: "Перечисление TextStrikeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.TextStrikeType. Этот тип определяет тип зачеркивания"
type: docs
url: /ru/net/aspose.cells/textstriketype/
---
## TextStrikeType enumeration

Этот тип указывает тип зачёркивания.

```csharp
public enum TextStrikeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Single | `0` | Одинарное зачеркивание, применяемое к тексту. |
| Double | `1` | Двойное зачеркивание, применяемое к тексту. Работает только для текста фигур или диаграмм. |
| None | `2` | К тексту не применяется зачеркивание. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextStrikeTypeDemo
    {
        public static void TextStrikeTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить ссылку на первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            // Доступ к ячейке "A1" листа
            Cell cell = worksheet.Cells["A1"];
            // Добавление некоторого значения в ячейку "A1"
            cell.PutValue("Hello Aspose!");

            // Доступ к шрифту ячейки
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Установка типа зачеркивания в Single
            font.StrikeType = TextStrikeType.Single;

            // Применить стиль к ячейке
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("TextStrikeTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


