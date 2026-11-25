---
title: "ExportTableOptions.RenameStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportTableOptions. Strategia per i nomi duplicati delle colonne"
type: docs
url: /it/net/aspose.cells/exporttableoptions/renamestrategy/
---
## ExportTableOptions.RenameStrategy property

Strategia per i nomi duplicati delle colonne.

```csharp
public RenameStrategy RenameStrategy { get; set; }
```

### Esempi

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

### Vedi anche

* enum [RenameStrategy](../../renamestrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


