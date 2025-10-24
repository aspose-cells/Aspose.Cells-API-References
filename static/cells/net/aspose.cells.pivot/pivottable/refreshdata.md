##PivotTable.RefreshData
PivotTable method. Refreshes pivottables data and setting from its data source
## RefreshData() {#refreshdata}
Refreshes pivottable's data and setting from it's data source.
```csharp
public PivotRefreshState RefreshData()
```
### Remarks
We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. This method is only used to gather all data to a pivot cache.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodRefreshDataDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(150);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row and data fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Refresh and calculate pivot table data
pivotTable.CalculateData();
pivotTable.RefreshData();
// Save the workbook
workbook.Save("PivotTableRefreshDataDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## RefreshData(PivotTableRefreshOption) {#refreshdata_1}
Refreshes pivottable's data and setting from it's data source with options.
```csharp
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```
| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The options for refreshing data source of pivot table. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Access the worksheet containing the pivot table
Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
// Get the first pivot table in the worksheet
PivotTable pivotTable = worksheet.PivotTables[0];
// Configure refresh options
PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
// Refresh the pivot table data with specified options
pivotTable.RefreshData(refreshOptions);
pivotTable.CalculateData();
// Save the modified workbook
workbook.Save("example_modified.xlsx");
}
}
}
```
### See Also
* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
