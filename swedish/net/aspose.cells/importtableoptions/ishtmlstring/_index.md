---
title: "ImportTableOptions.IsHtmlString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Anger om värdet innehåller html-taggar"
type: docs
url: /sv/net/aspose.cells/importtableoptions/ishtmlstring/
---
## ImportTableOptions.IsHtmlString property

Anger om värdet innehåller HTML‑taggar.

```csharp
public bool IsHtmlString { get; set; }
```

### Exempel

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
            // Skapa en DataTable med exempeldata som innehåller HTML
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Content");
            table.Columns.Add("Time");
            
            // Lägg till en rad med HTML-innehåll
            table.Rows.Add("1", "<a href='https://www.example.com'>Example Link</a>", "2:30 PM");

            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importera DataTable med IsHtmlString inställt på true
            worksheet.Cells.ImportData(table, 0, 0, new ImportTableOptions
            {
                IsFieldNameShown = true,
                IsHtmlString = true,
                NumberFormats = new string[] { null, null, "h:mm AM/PM" }
            });

            // Spara arbetsboken
            workbook.Save("HtmlStringImportDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


