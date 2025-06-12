---
title: ICellsDataTable.Columns
second_title: Aspose.Cells for .NET API Reference
description: ICellsDataTable property. Gets the columns name
type: docs
url: /net/aspose.cells/icellsdatatable/columns/
---
## ICellsDataTable.Columns property

Gets the columns' name.

```csharp
public string[] Columns { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ICellsDataTablePropertyColumnsDemo
    {
        public static void Run()
        {
            // Create workbook and access first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate headers and sample data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800.75);

            // Create data table from worksheet range with headers
            ExportTableOptions options = new ExportTableOptions { ExportColumnName = true };
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options);

            // Display initial columns
            Console.WriteLine("Original Columns:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.WriteLine(column.ColumnName);
            }

            // Modify headers in worksheet
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Cost");

            // Create new data table after header modification
            DataTable updatedDataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options);

            // Display updated columns
            Console.WriteLine("\nModified Columns:");
            foreach (DataColumn column in updatedDataTable.Columns)
            {
                Console.WriteLine(column.ColumnName);
            }

            // Demonstrate data iteration with current columns
            Console.WriteLine("\nData Contents:");
            foreach (DataRow row in updatedDataTable.Rows)
            {
                Console.WriteLine($"{row[0]}: {row[1]}");
            }

            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### See Also

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


