##PivotField.GetPivotFilters
PivotField method. Gets the pivot filters of the pivot field
## PivotField.GetPivotFilters method
Gets the pivot filters of the pivot field
```csharp
[Obsolete("Use PivotField.GetFilters() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetPivotFilters()
```
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.GetFilters() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
using System.Collections;
public class PivotFieldMethodGetPivotFiltersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["A5"].Value = "Apple";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 8;
worksheet.Cells["B5"].Value = 12;
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add pivot fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields[0];
try
{
// Call the GetPivotFilters method (obsolete)
ArrayList pivotFilters = pivotField.GetPivotFilters();
Console.WriteLine($"Number of pivot filters: {pivotFilters.Count}");
// Alternatively, use the non-obsolete GetFilters() method
PivotFilter[] filters = pivotField.GetFilters();
Console.WriteLine($"Number of filters (non-obsolete method): {filters.Length}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetPivotFilters method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetPivotFiltersDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
