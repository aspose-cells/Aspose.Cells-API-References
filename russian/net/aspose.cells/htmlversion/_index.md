---
title: "Перечисление HtmlVersion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.HtmlVersion. Указывает версию HTML, используемую при сохранении в форматы Html."
type: docs
url: /ru/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

Указывает версию HTML, используемую при сохранении в форматы HTML.

```csharp
public enum HtmlVersion
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Сохранить документ в соответствии с экспортом HTML из MS Excel. |
| XHtml | `1` | Сохраняет документ в соответствии со стандартом XHTML 1.0 Transitional. |
| Html5 | `2` | Сохраняет документ в соответствии со стандартом HTML 5. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Установить версию HTML в HTML5
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // Сохранить книгу с версией HTML5
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // Изменить версию HTML на XHTML
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // Сохранить книгу с версией XHTML
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // Установить версию HTML по умолчанию (совместимую с MS Excel)
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // Сохранить книгу с версией по умолчанию
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


