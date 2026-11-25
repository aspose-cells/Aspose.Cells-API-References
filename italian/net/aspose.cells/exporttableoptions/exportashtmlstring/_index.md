---
title: "ExportTableOptions.ExportAsHtmlString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportTableOptions. Esporta il valore stringa HTML delle celle nella DataTable"
type: docs
url: /it/net/aspose.cells/exporttableoptions/exportashtmlstring/
---
## ExportTableOptions.ExportAsHtmlString property

Esporta il valore stringa HTML delle celle nella DataTable.

```csharp
public bool ExportAsHtmlString { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsHtmlStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Imposta il valore della cella con formattazione
            cells["A1"].PutValue("abc");
            Style style = cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.Color = System.Drawing.Color.Black;
            cells["A1"].SetStyle(style);

            // Esporta con ExportAsHtmlString
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsHtmlString = true;
            
            DataTable dt = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            
            Console.WriteLine("HTML String: " + dt.Rows[0][0].ToString());
            Console.WriteLine("Expected Format: " + cells["A1"].HtmlString);
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


