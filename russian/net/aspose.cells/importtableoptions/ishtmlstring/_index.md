---
title: "ImportTableOptions.IsHtmlString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Указывает, содержит ли значение html‑теги."
type: docs
url: /ru/net/aspose.cells/importtableoptions/ishtmlstring/
---
## ImportTableOptions.IsHtmlString property

Указывает, содержит ли значение HTML‑теги.

```csharp
public bool IsHtmlString { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsHtmlStringDemo
    {
        public static void Run()
        {
            // Создать DataTable с примерными данными, содержащими HTML.
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Content");
            table.Columns.Add("Time");
            
            // Добавить строку с HTML‑содержимым.
            table.Rows.Add("1", "<a href='https://www.example.com'>Example Link</a>", "2:30 PM");

            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Импортировать DataTable с IsHtmlString, установленным в true.
            worksheet.Cells.ImportData(table, 0, 0, new ImportTableOptions
            {
                IsFieldNameShown = true,
                IsHtmlString = true,
                NumberFormats = new string[] { null, null, "h:mm AM/PM" }
            });

            // Сохраните книгу
            workbook.Save("HtmlStringImportDemo.xlsx");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


