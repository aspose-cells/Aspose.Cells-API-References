##PivotFieldSortSetting.FieldIndex
PivotFieldSortSetting property. Represents the index of the field sorted by. 1 means sorting the PivotField by the labelsothers means sorting by the data field
## PivotFieldSortSetting.FieldIndex property
Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field.
```csharp
public int FieldIndex { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldSortSettingPropertyFieldIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 5;
worksheet.Cells["B4"].Value = 8;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Get pivot field sort setting
PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
// Display current FieldIndex value
Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);
// Note: FieldIndex is read-only and PivotFieldSortSetting can't be instantiated directly
// as it has no public constructor. We can only work with the existing instance
// obtained from the pivot field's SortSetting property.
// Refresh pivot table to apply changes
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the result
workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
