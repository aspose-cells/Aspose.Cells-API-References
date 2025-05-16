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
namespace AsposeCellsExamples.CellsMethodImportGridViewWithGridViewInt32Int32ImportTableODemo
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportGridViewWithGridViewInt32Int32ImportTableODemo
    {
        public static void Run()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a DataTable with sample data
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            dataTable.Rows.Add(1, "John Doe", "Marketing");
            dataTable.Rows.Add(2, "Jane Smith", "Engineering");

            // Configure import options to include headers
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;

            try
            {
                // Import DataTable data into worksheet starting at cell (0,0)
                worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);
                
                Console.WriteLine("Data imported successfully. First cell value: " + 
                    worksheet.Cells[0, 0].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("ImportGridViewDemo.xlsx");
        }
    }
}
```

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


