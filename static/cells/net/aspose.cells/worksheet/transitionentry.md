##Worksheet.TransitionEntry
Worksheet property. Indicates whether the Transition Formula Entry Lotus compatibility option is enabled
## Worksheet.TransitionEntry property
Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.
```csharp
public bool TransitionEntry { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyTransitionEntryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set TransitionEntry property
worksheet.TransitionEntry = true;
// Display the TransitionEntry value
Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify the property
Workbook loadedWorkbook = new Workbook("output.xlsx");
Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
// Display the loaded TransitionEntry value
Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
