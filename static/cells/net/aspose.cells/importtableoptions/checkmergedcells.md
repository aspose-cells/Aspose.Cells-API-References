##ImportTableOptions.CheckMergedCells
ImportTableOptions property. Indicates whether checking merged cells
## ImportTableOptions.CheckMergedCells property
Indicates whether checking merged cells.
```csharp
public bool CheckMergedCells { get; set; }
```
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class Customer1
{
public int CustomerId { get; set; }
public string Name { get; set; }
}
public class ImportTableOptionsPropertyCheckMergedCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create merged cells for demonstration
worksheet.Cells.Merge(3, 3, 2, 1); // Merge D4:D5
worksheet.Cells[3, 3].PutValue("MergedValue");
// Create sample data
List<Customer1> customers = new List<Customer1>
{
new Customer1 { CustomerId = 1, Name = "Customer1" },
new Customer1 { CustomerId = 2, Name = "Customer2" },
new Customer1 { CustomerId = 3, Name = "Customer3" }
};
// Set import options with CheckMergedCells enabled
ImportTableOptions options = new ImportTableOptions
{
IsFieldNameShown = false,
InsertRows = true,
CheckMergedCells = true
};
// Import data
worksheet.Cells.ImportCustomObjects(customers, 0, 0, options);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
// Verify merged cells were preserved
Cell mergedCell = worksheet.Cells["D4"];
Console.WriteLine($"Merged cell value: {mergedCell.StringValue}");
Console.WriteLine($"Is cell merged: {mergedCell.IsMerged}");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
