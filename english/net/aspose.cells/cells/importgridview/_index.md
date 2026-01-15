---
title: Cells.ImportGridView
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports a grid view to this cells
type: docs
url: /net/aspose.cells/cells/importgridview/
---
## Cells.ImportGridView method

Imports a grid view to this cells.

```csharp
public int ImportGridView(GridView gridView, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| gridView | GridView | The grid view object. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| options | ImportTableOptions | import options. |

### Return Value

The row number.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a DataTable to simulate GridView data
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Price");
            dataTable.Columns.Add("Stock");

            dataTable.Rows.Add("Product A", 100.5, 50);
            dataTable.Rows.Add("Product B", 200.75, 30);
            dataTable.Rows.Add("Product C", 150.25, 75);

            try
            {
                // Create ImportTableOptions
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;
                options.InsertRows = true;

                // Import the DataTable data starting at cell B3 (row 2, column 1)
                worksheet.Cells.ImportData(dataTable, 2, 1, options);

                Console.WriteLine("Data imported successfully starting at cell B3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo.xlsx");
        }
    }
}
```

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


