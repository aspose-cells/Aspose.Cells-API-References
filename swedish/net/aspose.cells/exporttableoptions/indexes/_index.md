---
title: "ExportTableOptions.Indexes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions-egenskap. Indexen för kolumner/rader som ska exporteras"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/indexes/
---
## ExportTableOptions.Indexes property

Indexen för kolumner/rader som ska exporteras.

```csharp
public int[] Indexes { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIndexesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("Department");
            worksheet.Cells["D1"].PutValue("Salary");
            worksheet.Cells["E1"].PutValue("Join Date");
            
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["C2"].PutValue("IT");
            worksheet.Cells["D2"].PutValue(5000);
            worksheet.Cells["E2"].PutValue("2020-01-15");
            
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(28);
            worksheet.Cells["C3"].PutValue("HR");
            worksheet.Cells["D3"].PutValue(4500);
            worksheet.Cells["E3"].PutValue("2019-11-20");

            // Skapa exportalternativ och ange kolumnindex att exportera (i omvänd ordning)
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 4, 2, 0 }; // Export columns: Join Date, Department, Name

            // Exportera data med angivna kolumnindex
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 5, options);

            // Visa den exporterade datan
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
            }
        }
    }
}
```

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


