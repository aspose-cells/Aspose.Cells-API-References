##PivotTable.MoveTo
PivotTable method. Moves the PivotTable to a different location in the worksheet
## MoveTo(int, int) {#moveto}
Moves the PivotTable to a different location in the worksheet.
```csharp
public void MoveTo(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | row index. |
| column | Int32 | column index. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableMethodMoveToWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["A3"].PutValue("Vegetables");
worksheet.Cells["B1"].PutValue("Amount");
worksheet.Cells["B2"].PutValue(1500);
worksheet.Cells["B3"].PutValue(2500);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
// Calculate data to populate the pivot table
pivotTable.CalculateData();
try
{
// Call MoveTo method with (Int32, Int32) parameters to move the pivot table
pivotTable.MoveTo(5, 2); // Move to row 5, column 2
Console.WriteLine("Pivot table moved successfully to new location (5,2)");
// Calculate data again to update the moved pivot table
pivotTable.CalculateData();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing MoveTo method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableMethodMoveToWithInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## MoveTo(string) {#moveto_1}
Moves the PivotTable to a different location in the worksheet.
```csharp
public void MoveTo(string destCellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| destCellName | String | the dest cell name. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodMoveToWithStringDemo
{
public static void Run()
{
// Create a workbook
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
// Set sample data
cells["A1"].Value = "fruit";
cells["A2"].Value = "grape";
cells["A3"].Value = "blueberry";
cells["A4"].Value = "kiwi";
cells["A5"].Value = "cherry";
cells["A6"].Value = "grape";
cells["A7"].Value = "blueberry";
cells["A8"].Value = "kiwi";
cells["A9"].Value = "cherry";
cells["B1"].Value = "year";
cells["B2"].Value = 2020;
cells["B3"].Value = 2020;
cells["B4"].Value = 2020;
cells["B5"].Value = 2020;
cells["B6"].Value = 2021;
cells["B7"].Value = 2021;
cells["B8"].Value = 2021;
cells["B9"].Value = 2021;
cells["C1"].Value = "amount";
cells["C2"].Value = 50;
cells["C3"].Value = 60;
cells["C4"].Value = 70;
cells["C5"].Value = 80;
cells["C6"].Value = 90;
cells["C7"].Value = 100;
cells["C8"].Value = 110;
cells["C9"].Value = 120;
// Create pivot table
PivotTableCollection pivots = sheet.PivotTables;
int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
// Add fields to pivot table
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
// Set style and refresh
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
sheet.RefreshPivotTables();
// Move pivot table to new location
pivot.MoveTo("H16");
sheet.RefreshPivotTables();
// Save the workbook
book.Save("PivotTableMoveToExample.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
