##PivotItem.IsHideDetail
PivotItem property. Gets and sets whether the pivot item hides detail
## PivotItem.IsHideDetail property
Gets and sets whether the pivot item hides detail.
```csharp
[Obsolete("Use PivotItem.IsDetailHidden property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHideDetail { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotItem.IsDetailHidden property instead. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemPropertyIsHideDetailDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruit");
worksheet.Cells["A3"].PutValue("Vegetable");
worksheet.Cells["B1"].PutValue("Amount");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotField pivotField = pivotTable.RowFields[0];
PivotItemCollection pivotItems = pivotField.PivotItems;
foreach (PivotItem pivotItem in pivotItems)
{
Console.WriteLine($"Original IsHideDetail: {pivotItem.IsHideDetail}");
pivotItem.IsHideDetail = true;
Console.WriteLine($"Modified IsHideDetail: {pivotItem.IsHideDetail}");
}
workbook.Save("PivotItemIsHideDetailDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
