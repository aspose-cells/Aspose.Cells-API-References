---
title: Cells.DeleteColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes several columns
type: docs
url: /net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

Deletes several columns.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the first column to be deleted. |
| totalColumns | Int32 | Count of columns to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: ws.Cells.DeleteColumns(0, 1, true); // <-- This causes #REF too
public void Cells_Method_DeleteColumns()
{
    var file = Constants.sourcePath + @"example.xlsx";
    var wb = new Workbook(file);
    var ws = wb.Worksheets[0];
    // ws.Cells.InsertColumns(0, 4, true); // <-- This causes #REF 
    //ws.Cells.InsertColumns(0, 4); // <-- This causes #REF too
    ws.Cells.DeleteColumns(0, 1, true); // <-- This causes #REF too
    Assert.AreEqual("=SUBTOTAL(109,[Amount])",ws.Cells["C6"].Formula);

    wb = new Workbook(file);
    ws = wb.Worksheets[0];
    ws.Cells.InsertColumns(0, 4, true); // <-- This causes #REF 
    //ws.Cells.InsertColumns(0, 4); // <-- This causes #REF too
   // ws.Cells.DeleteColumns(0, 1, true); // <-- This causes #REF too
    Assert.AreEqual("=SUBTOTAL(109,[Amount])", ws.Cells["H6"].Formula);
    //wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

Deletes several columns.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the first column to be deleted. |
| totalColumns | Int32 | Count of columns to be deleted. |
| options | DeleteOptions | Options for the deleting operation |

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
{
    using Aspose.Cells;
    using System;

    public class CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Populate sample data in columns A-E
            for (int col = 0; col < 5; col++)
            {
                worksheet.Cells[0, col].Value = $"Column {(char)('A' + col)}";
                worksheet.Cells[1, col].Value = $"Data{col + 1}";
            }

            // Create DeleteOptions and configure settings
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Update references in other cells
            };

            try
            {
                // Delete 2 columns starting from column B (index 1)
                worksheet.Cells.DeleteColumns(1, 2, options);
                
                Console.WriteLine("Deleted columns B and C successfully");
                
                // Display remaining data in column B (original column D)
                Console.WriteLine($"New column B value: {worksheet.Cells[1, 1].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteColumns: {ex.Message}");
            }
            
            // Save the modified workbook
            workbook.Save("DeleteColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


