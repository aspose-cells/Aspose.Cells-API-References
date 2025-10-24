##Enum PivotRefreshState
Aspose.Cells.Pivot.PivotRefreshState enum. The state for refreshing pivot tables
## PivotRefreshState enumeration
The state for refreshing pivot tables.
```csharp
public enum PivotRefreshState
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Success | `0` | Successfully refreshed |
| UnsupportedExternalDataSource | `1` | Refresh failed because the data source is external. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotClassPivotRefreshStateDemo
{
public static void Run()
{
// Create a workbook with a sample pivot table
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
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Demonstrate PivotRefreshState
PivotRefreshState refreshState = pivotTable.RefreshData();
if (refreshState == PivotRefreshState.Success)
{
Console.WriteLine("Pivot table refreshed successfully");
}
else if (refreshState == PivotRefreshState.UnsupportedExternalDataSource)
{
Console.WriteLine("External data source not supported - calculating data instead");
pivotTable.CalculateData();
}
// Save the workbook
workbook.Save("PivotRefreshStateDemo_out.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
