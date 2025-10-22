##WorksheetCollection.RefreshPivotTables
WorksheetCollection method. Refreshes all the PivotTables in the Excel file
## RefreshPivotTables() {#refreshpivottables_1}
Refreshes all the PivotTables in the Excel file.
```csharp
public void RefreshPivotTables()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodRefreshPivotTablesDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B4"].PutValue(3000);
// Add pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);
// Modify source data
worksheet.Cells["B2"].PutValue(1500);
worksheet.Cells["B3"].PutValue(2500);
// Refresh all pivot tables in the workbook
workbook.Worksheets.RefreshPivotTables();
// Save the workbook
workbook.Save("RefreshPivotTablesDemo.xlsx");
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}
Refreshes all the PivotTables in the Excel file.
```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```
| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of the pivot tables. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
cells["A1"].Value = "Category";
cells["A2"].Value = "Fruit";
cells["A3"].Value = "Vegetable";
cells["B1"].Value = "Sales";
cells["B2"].Value = 1500;
cells["B3"].Value = 2300;
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B3", "E5", "SalesPivot");
PivotTable pivotTable = pivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotTableRefreshOption option = new PivotTableRefreshOption();
workbook.Worksheets.RefreshPivotTables(option);
Console.WriteLine(cells["F8"].StringValue);
cells["B2"].Value = 2000;
workbook.Worksheets.RefreshPivotTables(option);
Console.WriteLine(cells["F8"].StringValue);
workbook.Save("WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
