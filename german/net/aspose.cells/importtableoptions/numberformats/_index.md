---
title: "ImportTableOptions.NumberFormats"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Ruft die Zahlenformate ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells/importtableoptions/numberformats/
---
## ImportTableOptions.NumberFormats property

Liest oder legt die Zahlenformate fest

```csharp
public string[] NumberFormats { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyNumberFormatsDemo
    {
        public static void Run()
        {
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Description");
            table.Columns.Add("TimeValue");
            
            table.Rows.Add(1, "Sample Item 1", DateTime.Parse("1:30 PM"));
            table.Rows.Add(2, "Sample Item 2", DateTime.Parse("3:45 PM"));

            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            var importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                NumberFormats = new string[] { null, null, "h:mm AM/PM" }
            };

            worksheet.Cells.ImportData(table, 0, 0, importOptions);
            
            workbook.Save("NumberFormatsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


