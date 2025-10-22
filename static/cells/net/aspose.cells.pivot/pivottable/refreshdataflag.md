##PivotTable.RefreshDataFlag
PivotTable property. Indicates whether Refreshing Data or not
## PivotTable.RefreshDataFlag property
Indicates whether Refreshing Data or not.
```csharp
[Obsolete("Simply remove this calling.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool RefreshDataFlag { get; set; }
```
### Remarks
NOTE: This method is now obsolete. Instead, This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyRefreshDataFlagDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Region");
worksheet.Cells["C1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["B2"].PutValue("North");
worksheet.Cells["C2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B3"].PutValue("South");
worksheet.Cells["C3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Product C");
worksheet.Cells["B4"].PutValue("East");
worksheet.Cells["C4"].PutValue(3000);
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("=A1:C4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current RefreshDataFlag value
Console.WriteLine("Current RefreshDataFlag value: " + pivotTable.RefreshDataFlag);
// Set RefreshDataFlag to false to prevent auto-refresh
pivotTable.RefreshDataFlag = false;
// Change the source data
worksheet.Cells["C2"].PutValue(5000);
// Refresh the pivot table manually since RefreshDataFlag is false
pivotTable.RefreshData();
// Save the workbook
workbook.Save("PivotTablePropertyRefreshDataFlagDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
