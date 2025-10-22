##Worksheet.GetSelectedAreas
Worksheet method. Gets selected ranges of cells in the designer spreadsheet
## Worksheet.GetSelectedAreas method
Gets selected ranges of cells in the designer spreadsheet.
```csharp
public Range[] GetSelectedAreas()
```
### Return Value
Returns all selected ranges.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodGetSelectedAreasDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Select multiple ranges
worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
// Get selected areas
Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
// Display information about selected areas
Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
for (int i = 0; i < selectedAreas.Length; i++)
{
Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
}
// Clear selections and select a single range
worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
// Get the single selected area
selectedAreas = worksheet.GetSelectedAreas();
Console.WriteLine("\nAfter single selection:");
Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
Console.WriteLine("Selected area: " + selectedAreas[0].Address);
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
