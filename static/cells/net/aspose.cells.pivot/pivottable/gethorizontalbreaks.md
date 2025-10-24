##PivotTable.GetHorizontalBreaks
PivotTable method. Gets pivot table row index list of horizontal page breaks
## PivotTable.GetHorizontalBreaks method
Gets pivot table row index list of horizontal page breaks
```csharp
[Obsolete("Use ivotTable.GetHorizontalPageBreaks() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetHorizontalBreaks()
```
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotTable.GetHorizontalPageBreaks() method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
using System.Collections;
public class PivotTableMethodGetHorizontalBreaksDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["A5"].PutValue("Grape");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
worksheet.Cells["B5"].PutValue(4000);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Calculate data to populate the pivot table
pivotTable.CalculateData();
try
{
// Get horizontal breaks (page breaks) for the pivot table
ArrayList horizontalBreaks = pivotTable.GetHorizontalBreaks();
Console.WriteLine("Horizontal breaks (row indices):");
foreach (int rowIndex in horizontalBreaks)
{
Console.WriteLine(rowIndex);
}
// Add a page break at row 3 for demonstration
worksheet.HorizontalPageBreaks.Add("A3");
// Get updated horizontal breaks
horizontalBreaks = pivotTable.GetHorizontalBreaks();
Console.WriteLine("\nHorizontal breaks after adding page break:");
foreach (int rowIndex in horizontalBreaks)
{
Console.WriteLine(rowIndex);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetHorizontalBreaks method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableGetHorizontalBreaksDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
