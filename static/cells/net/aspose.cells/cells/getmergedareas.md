##Cells.GetMergedAreas
Cells method. Gets all merged cells
## Cells.GetMergedAreas method
Gets all merged cells.
```csharp
public CellArea[] GetMergedAreas()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetMergedAreasDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create some merged cells
worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
// Get all merged areas
CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
// Display information about merged areas
Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
foreach (CellArea area in mergedAreas)
{
Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
$"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
}
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
