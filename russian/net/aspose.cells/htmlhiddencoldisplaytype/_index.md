---
title: "Перечисление HtmlHiddenColDisplayType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.HtmlHiddenColDisplayType. Представляет два типа отображения скрытых столбцов в HTML"
type: docs
url: /ru/net/aspose.cells/htmlhiddencoldisplaytype/
---
## HtmlHiddenColDisplayType enumeration

Представляет два типа отображения скрытых столбцов в HTML.

```csharp
public enum HtmlHiddenColDisplayType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Hidden | `0` | Скрыть скрытые столбцы на HTML-странице. |
| Remove | `1` | Удалить скрытые столбцы на HTML-странице. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenColDisplayTypeDemo
    {
        public static void HtmlHiddenColDisplayTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Скрыть второй столбец
            worksheet.Cells.HideColumn(1);

            // Создайте HtmlSaveOptions и установите HiddenColDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;

            // Сохраните книгу в формате HTML
            workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


