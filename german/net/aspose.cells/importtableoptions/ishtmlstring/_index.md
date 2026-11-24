---
title: "ImportTableOptions.IsHtmlString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions Eigenschaft. Gibt an, ob der Wert HTML‑Tags enthält"
type: docs
url: /de/net/aspose.cells/importtableoptions/ishtmlstring/
---
## ImportTableOptions.IsHtmlString property

Gibt an, ob der Wert HTML‑Tags enthält.

```csharp
public bool IsHtmlString { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine DataTable mit Beispieldaten, die HTML enthalten
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Content");
            table.Columns.Add("Time");
            
            // Fügen Sie eine Zeile mit HTML‑Inhalt hinzu
            table.Rows.Add("1", "<a href='https://www.example.com'>Example Link</a>", "2:30 PM");

            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importieren Sie die DataTable mit IsHtmlString auf true gesetzt
            worksheet.Cells.ImportData(table, 0, 0, new ImportTableOptions
            {
                IsFieldNameShown = true,
                IsHtmlString = true,
                NumberFormats = new string[] { null, null, "h:mm AM/PM" }
            });

            // Speichere die Arbeitsmappe
            workbook.Save("HtmlStringImportDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


