##Worksheet.RefreshPivotTables
Worksheet method. Refreshes all the PivotTables in this Worksheet
## RefreshPivotTables() {#refreshpivottables_1}
Refreshes all the PivotTables in this Worksheet.
```csharp
public void RefreshPivotTables()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodRefreshPivotTablesDemo
{
public static void Run()
{
// Create a workbook from source Excel file containing pivot tables
Workbook workbook = new Workbook("example.xlsx");
// Get the first worksheet which contains pivot tables
Worksheet worksheet = workbook.Worksheets[0];
// Refresh all pivot tables in the worksheet
worksheet.RefreshPivotTables();
// Save the updated workbook
workbook.Save("RefreshedPivotTables.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}
Refreshes all the PivotTables in this Worksheet.
```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```
| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of pivot table. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
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
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 20;
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
worksheet.RefreshPivotTables();
int preCount = pivotTable.RowFields[0].PivotItems.Count;
// Modify source data
worksheet.Cells["A2"].Value = "test2";
worksheet.Cells["A3"].Value = "test3";
// Create refresh options
PivotTableRefreshOption options = new PivotTableRefreshOption
{
ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
};
worksheet.RefreshPivotTables(options);
int nowCount = pivotTable.RowFields[0].PivotItems.Count;
Console.WriteLine(nowCount > preCount);
// Save the result
workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
