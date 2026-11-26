---
title: "Перечисление FontSchemeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.FontSchemeType. Представляет тип схемы шрифта."
type: docs
url: /ru/net/aspose.cells/fontschemetype/
---
## FontSchemeType enumeration

Представляет тип схемы шрифта.

```csharp
public enum FontSchemeType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет |
| Major | `1` | Основная схема. |
| Minor | `2` | Вторичная схема. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSchemeTypeDemo
    {
        public static void FontSchemeTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить ссылку на первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            // Доступ к ячейке "A1" листа
            Cell cell = worksheet.Cells["A1"];
            // Добавление некоторого значения в ячейку "A1"
            cell.PutValue("Hello Aspose!");

            // Получить доступ к шрифту стиля ячейки
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Установка типа схемы шрифта в Major
            font.SchemeType = FontSchemeType.Major;

            // Установка других свойств шрифта для демонстрации
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // Сохраните книгу
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


