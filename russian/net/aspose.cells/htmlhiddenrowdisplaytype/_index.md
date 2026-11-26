---
title: "Перечисление HtmlHiddenRowDisplayType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.HtmlHiddenRowDisplayType. Представляет два типа отображения скрытых строк в html"
type: docs
url: /ru/net/aspose.cells/htmlhiddenrowdisplaytype/
---
## HtmlHiddenRowDisplayType enumeration

Представляет два типа отображения скрытых строк в HTML.

```csharp
public enum HtmlHiddenRowDisplayType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Hidden | `0` | Скрыть скрытые строки на странице html. |
| Remove | `1` | Удалить скрытые строки на странице html. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenRowDisplayTypeDemo
    {
        public static void HtmlHiddenRowDisplayTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Another Visible Row");

            // Скрыть вторую строку
            worksheet.Cells.HideRow(1);

            // Создать HtmlSaveOptions и установить HiddenRowDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove

            // Сохраните книгу в формате HTML
            workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden row display type.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


