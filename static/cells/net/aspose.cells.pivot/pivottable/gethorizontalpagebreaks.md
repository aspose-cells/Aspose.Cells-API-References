##PivotTable.GetHorizontalPageBreaks
PivotTable method. Gets horizontal page breaks of this pivot table
## PivotTable.GetHorizontalPageBreaks method
Gets horizontal page breaks of this pivot table.
```csharp
public int[] GetHorizontalPageBreaks()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodGetHorizontalPageBreaksDemo
{
public static void Run()
{
// Create a workbook from source file
Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the first pivot table
PivotTable pivotTable = worksheet.PivotTables[0];
// Refresh and calculate pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Get horizontal page breaks
int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
// Display the results
Console.WriteLine("Horizontal Page Breaks:");
foreach (int row in pageBreaks)
{
Console.WriteLine("Row: " + row);
}
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
