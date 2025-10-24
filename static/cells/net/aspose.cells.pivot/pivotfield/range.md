##PivotField.Range
PivotField property. Gets the group range of the pivot field
## PivotField.Range property
Gets the group range of the pivot field
```csharp
[Obsolete("Use PivotField.GroupSettings property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SxRng Range { get; }
```
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.GroupSettings property. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyRangeDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 300;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Access the row field
PivotField rowField = pivotTable.RowFields[0];
// Access and display range properties
SxRng range = rowField.Range;
Console.WriteLine("Range Properties:");
Console.WriteLine($"IsAutoStart: {range.IsAutoStart}");
Console.WriteLine($"IsAutoEnd: {range.IsAutoEnd}");
Console.WriteLine($"Start: {range.Start}");
Console.WriteLine($"End: {range.End}");
Console.WriteLine($"By: {range.By}");
// Save the workbook
workbook.Save("PivotFieldRangeDemo.xlsx");
}
}
}
```
### See Also
* class [SxRng](../../sxrng/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
