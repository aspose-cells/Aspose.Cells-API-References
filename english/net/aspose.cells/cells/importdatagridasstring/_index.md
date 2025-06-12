---
title: Cells.ImportDataGridAsString
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports a DataGrid into a worksheet. This method doesnt try to convert text into numeric values
type: docs
url: /net/aspose.cells/cells/importdatagridasstring/
---
## Cells.ImportDataGridAsString method

Imports a DataGrid into a worksheet. This method doesn't try to convert text into numeric values.

```csharp
public int ImportDataGridAsString(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataGrid | DataGrid | The DataGrid object to be imported. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |

### Return Value

Total number of rows imported

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportDataGridAsStringWithDataGridInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create and populate DataTable
            DataTable table = new DataTable();
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Age", typeof(int));
            table.Rows.Add("John Doe", 30);
            table.Rows.Add("Jane Smith", 28);

            try
            {
                // Create ImportTableOptions with required settings
                ImportTableOptions options = new ImportTableOptions
                {
                    IsFieldNameShown = true,
                    ConvertNumericData = true // Corrected property name
                };

                // Call ImportData with parameters: DataTable, row=0, column=0, options
                int importedRows = worksheet.Cells.ImportData(table, 0, 0, options);

                Console.WriteLine($"Successfully imported {importedRows} rows from DataTable");
                Console.WriteLine($"Data starts at: A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData: {ex.Message}");
            }

            // Save the result
            workbook.Save("ImportDataGridAsStringDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


