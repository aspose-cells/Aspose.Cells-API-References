##TableStyleCollection.AddPivotTableStyle
TableStyleCollection method. Adds a custom pivot table style
## TableStyleCollection.AddPivotTableStyle method
Adds a custom pivot table style.
```csharp
public int AddPivotTableStyle(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The pivot table style name. |
### Return Value
The index of the pivot table style.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableStyleCollectionMethodAddPivotTableStyleWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Region");
worksheet.Cells["C1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue("North");
worksheet.Cells["C2"].PutValue(1200);
worksheet.Cells["A3"].PutValue("Desktop");
worksheet.Cells["B3"].PutValue("South");
worksheet.Cells["C3"].PutValue(800);
worksheet.Cells["A4"].PutValue("Tablet");
worksheet.Cells["B4"].PutValue("East");
worksheet.Cells["C4"].PutValue(500);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 1);
pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);
try
{
// Get the table style collection
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
// Call AddPivotTableStyle with String parameter
int styleIndex = tableStyles.AddPivotTableStyle("CustomPivotStyle1");
Console.WriteLine($"Added pivot table style at index: {styleIndex}");
// Set the new style as default pivot style
tableStyles.DefaultPivotStyleName = "CustomPivotStyle1";
// Apply the style to our pivot table
pivotTable.PivotTableStyleName = "CustomPivotStyle1";
Console.WriteLine("Applied custom pivot table style successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AddPivotTableStyle method: {ex.Message}");
}
// Save the workbook
workbook.Save("TableStyleCollectionMethodAddPivotTableStyleWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
