---
title: "Перечисление HtmlExportDataOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.HtmlExportDataOptions. Представляет параметры экспорта HTML-данных."
type: docs
url: /ru/net/aspose.cells/htmlexportdataoptions/
---
## HtmlExportDataOptions enumeration

Представляет параметры экспорта HTML‑данных.

```csharp
public enum HtmlExportDataOptions
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Table | `1` | Экспортировать файл в HTML, содержащий только часть таблицы. |
| All | `255` | Экспортировать все данные в HTML. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlExportDataOptionsDemo
    {
        public static void HtmlExportDataOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Doe");
            worksheet.Cells["B3"].PutValue(25);

            // Создать HtmlSaveOptions и установить HtmlExportDataOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML

            // Сохраните книгу в формате HTML
            workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);

            // Изменить HtmlExportDataOptions для экспорта только части таблицы
            saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part

            // Сохранить книгу в формате HTML снова
            workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);

            Console.WriteLine("HTML files have been saved successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


