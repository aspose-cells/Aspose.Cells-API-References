---
title: "ExportTableOptions.ExportAsHtmlString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions egenskap. Exporterar cellernas HTML-strängvärde till DataTable"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/exportashtmlstring/
---
## ExportTableOptions.ExportAsHtmlString property

Exporterar cellernas HTML-strängvärde till DataTable.

```csharp
public bool ExportAsHtmlString { get; set; }
```

### Exempel

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
            
            // Ange cellvärde med formatering
            cells["A1"].PutValue("abc");
            Style style = cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.Color = System.Drawing.Color.Black;
            cells["A1"].SetStyle(style);

            // Exportera med ExportAsHtmlString
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

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


