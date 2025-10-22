##PivotField.BaseItemIndex
PivotField property. Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields
## PivotField.BaseItemIndex property
Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields.
```csharp
[Obsolete("Use PivotField.ShowValuesSetting.BaseItemIndex property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int BaseItemIndex { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyBaseItemIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].Value = "Category";
cells["A2"].Value = "Fruit";
cells["A3"].Value = "Fruit";
cells["A4"].Value = "Vegetable";
cells["A5"].Value = "Vegetable";
cells["B1"].Value = "Item";
cells["B2"].Value = "Apple";
cells["B3"].Value = "Orange";
cells["B4"].Value = "Carrot";
cells["B5"].Value = "Potato";
cells["C1"].Value = "Sales";
cells["C2"].Value = 100;
cells["C3"].Value = 150;
cells["C4"].Value = 200;
cells["C5"].Value = 250;
// Create pivot table and get its index
int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get the first row field (Category)
PivotField rowField = pivotTable.RowFields[0];
// Set BaseItemIndex to show difference from first item
rowField.BaseFieldIndex = 0;
rowField.BaseItemIndex = 0;
rowField.DataDisplayFormat = PivotFieldDataDisplayFormat.DifferenceFrom;
// Refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldBaseItemIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
