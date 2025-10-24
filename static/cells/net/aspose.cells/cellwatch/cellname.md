##CellWatch.CellName
CellWatch property. Gets and sets the name of the cell
## CellWatch.CellName property
Gets and sets the name of the cell.
```csharp
public string CellName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellWatchPropertyCellNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some cell watches
worksheet.CellWatches.Add("B5");
worksheet.CellWatches.Add("C10");
// Display cell names of all watches
Console.WriteLine("Cell Watches:");
foreach (CellWatch watch in worksheet.CellWatches)
{
Console.WriteLine(watch.CellName);
}
// Add a new watch and display its name
worksheet.CellWatches.Add("A1");
Console.WriteLine("Added new watch: " +
worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
// Save the workbook
workbook.Save("CellWatchDemo.xlsx");
}
}
}
```
### See Also
* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
