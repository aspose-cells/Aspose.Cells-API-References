---
title: "Перечисление HtmlLinkTargetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.HtmlLinkTargetType. Представляет тип атрибута target в HTML‑теге"
type: docs
url: /ru/net/aspose.cells/htmllinktargettype/
---
## HtmlLinkTargetType enumeration

Представляет тип атрибута target в теге HTML.

```csharp
public enum HtmlLinkTargetType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Blank | `0` | Открывает связанный документ в новом окне или вкладке |
| Parent | `1` | Открывает связанный документ в родительском фрейме |
| Self | `2` | Открывает связанный документ в том же фрейме, в котором был щёлкнут (это значение по умолчанию) |
| Top | `3` | Открывает связанный документ в полном теле окна |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLinkTargetTypeDemo
    {
        public static void HtmlLinkTargetTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Создать HtmlSaveOptions и установить LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // Сохраните книгу в формате HTML
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


