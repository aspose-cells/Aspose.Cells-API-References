---
title: "ICellsDataTable.Columns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ICellsDataTable egenskap. Hämtar kolumnnamnet"
type: docs
url: /sv/net/aspose.cells/icellsdatatable/columns/
---
## ICellsDataTable.Columns property

Hämtar kolumnens namn.

```csharp
public string[] Columns { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyColumnsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["C1"].PutValue("Stock");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["C2"].PutValue(15);

            try
            {
                // Exportera dataområde till ICellsDataTable
                ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 2, 3);

                // Visa kolumnnamnen
                Console.WriteLine("Column names in the data table:");
                foreach (string column in dataTable.Columns)
                {
                    Console.WriteLine(column);
                }

                // Visa antalet kolumner
                Console.WriteLine($"Total columns: {dataTable.Columns.Length}");

                // Spara arbetsboken
                workbook.Save("ColumnsDemo.xlsx");
                Console.WriteLine("Columns property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


