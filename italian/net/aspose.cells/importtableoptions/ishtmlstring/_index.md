---
title: "ImportTableOptions.IsHtmlString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Indica se il valore contiene tag HTML"
type: docs
url: /it/net/aspose.cells/importtableoptions/ishtmlstring/
---
## ImportTableOptions.IsHtmlString property

Indica se il valore contiene tag HTML.

```csharp
public bool IsHtmlString { get; set; }
```

### Esempi

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
            // Crea un DataTable con dati di esempio contenenti HTML
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Content");
            table.Columns.Add("Time");
            
            // Aggiungi una riga con contenuto HTML
            table.Rows.Add("1", "<a href='https://www.example.com'>Example Link</a>", "2:30 PM");

            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importa il DataTable con IsHtmlString impostato su true
            worksheet.Cells.ImportData(table, 0, 0, new ImportTableOptions
            {
                IsFieldNameShown = true,
                IsHtmlString = true,
                NumberFormats = new string[] { null, null, "h:mm AM/PM" }
            });

            // Salva la cartella di lavoro
            workbook.Save("HtmlStringImportDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


