##PivotFieldSortSetting.IsSimpleSort
PivotFieldSortSetting property. Indicates whether a simple data sort operation will be applied
## PivotFieldSortSetting.IsSimpleSort property
Indicates whether a simple data sort operation will be applied.
```csharp
public bool IsSimpleSort { get; }
```
### Remarks
The default value is true.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldSortSettingPropertyIsSimpleSortDemo
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
worksheet.Cells["A5"].Value = "Apple";
worksheet.Cells["A6"].Value = "Orange";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 300;
worksheet.Cells["B5"].Value = 150;
worksheet.Cells["B6"].Value = 250;
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get pivot field
PivotField pivotField = pivotTable.RowFields[0];
// Get sort setting (read-only property)
PivotFieldSortSetting sortSetting = pivotField.SortSetting;
// Display current IsSimpleSort value
Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);
// Note: IsSimpleSort is read-only, so we cannot set it directly
// To demonstrate sorting, we'll create a new pivot table with different sorting
// Create another pivot table with custom sort
pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
PivotTable pivotTable2 = pivotTables[pivotIndex];
pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");
// Sort the pivot field using available method
PivotField pivotField2 = pivotTable2.RowFields[0];
pivotField2.SortBy(SortOrder.Ascending, -1);
// Save the workbook
workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
