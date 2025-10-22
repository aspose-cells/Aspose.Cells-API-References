##Worksheet.ActiveCell
Worksheet property. Gets or sets the active cell in the worksheet
## Worksheet.ActiveCell property
Gets or sets the active cell in the worksheet.
```csharp
public string ActiveCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyActiveCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set active cell to B2
worksheet.ActiveCell = "B2";
// Print active cell address
Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify active cell
Workbook loadedWorkbook = new Workbook("output.xlsx");
Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
