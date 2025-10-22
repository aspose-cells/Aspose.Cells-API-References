##PivotField.BaseItemPosition
PivotField property. Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for readif you need to set PivotItemPosition.Custom please set PivotField.BaseItemIndex attribute
## PivotField.BaseItemPosition property
Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.
```csharp
[Obsolete("Use PivotField.ShowValuesSetting.BaseItemPositionType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotItemPosition BaseItemPosition { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseItemPositionType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyBaseItemPositionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "A";
worksheet.Cells["A3"].Value = "B";
worksheet.Cells["A4"].Value = "A";
worksheet.Cells["B1"].Value = "Value";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 20;
worksheet.Cells["B4"].Value = 30;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value
// Configure base item position
PivotField categoryField = pivotTable.RowFields[0];
categoryField.BaseItemPosition = PivotItemPosition.Next;
// Calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
workbook.Save("PivotFieldBaseItemPositionDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotItemPosition](../../pivotitemposition/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
