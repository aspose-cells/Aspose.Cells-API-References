##Enum ReserveMissingPivotItemType
Aspose.Cells.Pivot.ReserveMissingPivotItemType enum. Represents how to keep the missing pivot items
## ReserveMissingPivotItemType enumeration
Represents how to keep the missing pivot items.
```csharp
public enum ReserveMissingPivotItemType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Removes old missint pivot items and reserves visible items which the current data source does not contain as missing items. |
| All | `1` | Reserves all missing items. |
| None | `2` | Removes all missing pivot items. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class ReserveMissingPivotItemTypeDemo
{
public static void ReserveMissingPivotItemTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a PivotTable to the worksheet
int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
// Add fields to the PivotTable
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Set the ReserveMissingPivotItemType option
PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
{
RefreshData = true,
RefreshCharts = true,
ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
};
// Calculate the PivotTable with the specified options
pivotTable.CalculateData(calculateOption);
// Refresh the PivotTable
pivotTable.RefreshData();
// Save the workbook
workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
