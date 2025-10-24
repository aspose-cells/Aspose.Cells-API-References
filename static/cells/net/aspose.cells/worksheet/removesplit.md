##Worksheet.RemoveSplit
Worksheet method. Removes split window
## Worksheet.RemoveSplit method
Removes split window.
```csharp
public void RemoveSplit()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodRemoveSplitDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Split the worksheet
worksheet.Split();
Console.WriteLine("Worksheet split state: " + worksheet.PaneState);
// Remove the split
worksheet.RemoveSplit();
Console.WriteLine("Worksheet split state after RemoveSplit: " + worksheet.PaneState);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
