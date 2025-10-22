##Style.IsJustifyDistributed
Style property. Indicates if the cells justified or distributed alignment should be used on the last line of text
## Style.IsJustifyDistributed property
Indicates if the cells justified or distributed alignment should be used on the last line of text.
```csharp
public bool IsJustifyDistributed { get; set; }
```
### Remarks
This is typical for East Asian alignments but not typical in other contexts.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsJustifyDistributedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B3 and set its text
Cell cell = worksheet.Cells["B3"];
cell.PutValue("Sample Text");
// Get the cell's style and set IsJustifyDistributed to true
Style style = cell.GetStyle();
style.IsJustifyDistributed = true;
cell.SetStyle(style);
// Save the workbook
workbook.Save("output.xlsx");
// Verify the property
Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
