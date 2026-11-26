---
title: "Перечисление JsonExportHyperlinkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Json.JsonExportHyperlinkType. Представляет тип экспорта гиперссылок в json"
type: docs
url: /ru/net/aspose.cells.json/jsonexporthyperlinktype/
---
## JsonExportHyperlinkType enumeration

Представляет тип, определяющий, как экспортировать гиперссылки в JSON.

```csharp
public enum JsonExportHyperlinkType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DisplayString | `0` | Экспортировать отображаемую строку |
| Address | `1` | Экспортировать URL |
| HtmlString | `2` | Экспортировать как HTML-строку. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonExportHyperlinkTypeDemo
    {
        public static void JsonExportHyperlinkTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные с гиперссылками
            worksheet.Cells["A1"].PutValue("Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");

            worksheet.Cells["A2"].PutValue("Aspose");
            worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");

            // Создать JsonSaveOptions и установить ExportHyperlinkType
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;

            // Сохранить книгу в формате JSON
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);

            // Измените ExportHyperlinkType на Address и сохраните снова
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);

            // Измените ExportHyperlinkType на HtmlString и сохраните снова
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);

            Console.WriteLine("Workbooks saved with different hyperlink export types.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)


