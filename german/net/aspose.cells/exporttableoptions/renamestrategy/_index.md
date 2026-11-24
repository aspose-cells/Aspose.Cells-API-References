---
title: "ExportTableOptions.RenameStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions-Eigenschaft. Strategie für doppelte Spaltennamen"
type: docs
url: /de/net/aspose.cells/exporttableoptions/renamestrategy/
---
## ExportTableOptions.RenameStrategy property

Strategie für doppelte Spaltennamen.

```csharp
public RenameStrategy RenameStrategy { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyRenameStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit
            };

            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            Console.WriteLine("Exported DataTable with Digit RenameStrategy:");
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row[0]);
            }

            workbook.Save("RenameStrategyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RenameStrategy](../../renamestrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


