##Cells.PreserveString
Cells property. Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false
## Cells.PreserveString property
Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false.
```csharp
public bool PreserveString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyPreserveStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set PreserveString property to true
cells.PreserveString = true;
// Add string values to cells
cells["A1"].PutValue("Preserved String 1");
cells["B1"].PutValue("Preserved String 2");
// Access the values (they will be preserved as strings)
Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);
// Save the workbook
workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);
// Load the saved workbook to verify preservation
Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
// Output the preserved values
Console.WriteLine("\nAfter loading:");
Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);
// Demonstrate PreserveString property comparison
Console.WriteLine("\nPreserveString property matches: " +
(cells.PreserveString == loadedCells.PreserveString));
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
