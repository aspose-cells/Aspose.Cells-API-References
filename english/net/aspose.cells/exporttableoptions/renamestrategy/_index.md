---
title: ExportTableOptions.RenameStrategy
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Strategy for duplicate names of columns
type: docs
url: /net/aspose.cells/exporttableoptions/renamestrategy/
---
## ExportTableOptions.RenameStrategy property

Strategy for duplicate names of columns.

```csharp
public RenameStrategy RenameStrategy { get; set; }
```

### Examples

```csharp
// Called: RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
public static void ExportTableOptions_Property_RenameStrategy()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // Create ExportTableOptions and set the RenameStrategy
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // Export the worksheet data to a DataTable
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // Display the DataTable content
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Save the workbook
            workbook.Save("RenameStrategyExample.xlsx");
        }
```

### See Also

* enum [RenameStrategy](../../renamestrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


