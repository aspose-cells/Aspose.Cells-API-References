##Cell.IsCheckBoxStyle
Cell property. Indicates whether setting this cell as a check box
## Cell.IsCheckBoxStyle property
Indicates whether setting this cell as a check box.
```csharp
public bool IsCheckBoxStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyIsCheckBoxStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B1 and set it to checkbox style
Cell cell = worksheet.Cells["B1"];
cell.IsCheckBoxStyle = true;
cell.PutValue(true);
// Access cell A1 and set it to checkbox style with a value
cell = worksheet.Cells["A1"];
cell.IsCheckBoxStyle = true;
cell.PutValue(false);
// Save the workbook
workbook.Save("CheckBoxStyleDemo.xlsx");
// Load the saved workbook to verify properties
Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
worksheet = loadedWorkbook.Worksheets[0];
// Verify B1 is checkbox style
cell = worksheet.Cells["B1"];
Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
// Change B1 to non-checkbox style and save
cell.IsCheckBoxStyle = false;
loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
