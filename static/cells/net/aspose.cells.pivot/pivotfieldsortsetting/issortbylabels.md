##PivotFieldSortSetting.IsSortByLabels
PivotFieldSortSetting property. Indicates whether sorting the field by itself or data field
## PivotFieldSortSetting.IsSortByLabels property
Indicates whether sorting the field by itself or data field.
```csharp
public bool IsSortByLabels { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldSortSettingPropertyIsSortByLabelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = worksheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 20;
cells["A4"].Value = "Banana";
cells["B4"].Value = 15;
cells["A5"].Value = "Apple";
cells["B5"].Value = 5;
cells["A6"].Value = "Orange";
cells["B6"].Value = 10;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Get pivot field sort setting
PivotField pivotField = pivotTable.RowFields[0];
PivotFieldSortSetting sortSetting = pivotField.SortSetting;
// Display current IsSortByLabels value
Console.WriteLine("Current IsSortByLabels value: " + sortSetting.IsSortByLabels);
// Note: IsSortByLabels is read-only, so we can't set it directly
// Instead, we'll demonstrate its meaning by examining the sort settings
// Show related sort properties
Console.WriteLine("SortType: " + sortSetting.SortType);
Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
// Save the workbook
workbook.Save("PivotFieldSortSettingPropertyIsSortByLabelsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
