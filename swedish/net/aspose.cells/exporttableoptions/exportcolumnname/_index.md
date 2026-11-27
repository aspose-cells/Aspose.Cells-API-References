---
title: "ExportTableOptions.ExportColumnName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions-egenskap. Anger om data i den första raden exporteras till kolumnnamnet i DataTable. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

Indikerar om data i den första raden exporteras till kolumnnamnet i DataTable. Standardvärdet är false.

```csharp
public bool ExportColumnName { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportColumnNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempeldata i kalkylbladet
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Data1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Data2");

            // Konfigurera exportalternativ
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true; // Demonstrating ExportColumnName property
            options.IsVertical = true;
            options.Indexes = new int[] { 0, 1 }; // Export all columns

            // Exportera data från kalkylblad till DataTable
            DataTable dataTable = cells.ExportDataTable(0, 0, 4, 2, options);

            // Visa exporterad data
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Column1"]}, {row["Column2"]}");
            }
        }
    }
}
```

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


