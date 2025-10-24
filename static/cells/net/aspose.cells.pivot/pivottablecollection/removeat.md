##PivotTableCollection.RemoveAt
PivotTableCollection method. Deletes the PivotTable at the specified index and delete the PivotTable data
## RemoveAt(int) {#removeat}
Deletes the PivotTable at the specified index and delete the PivotTable data
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the position index in PivotTable collection |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PivotTableCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(100);
sheet.Cells["B3"].PutValue(200);
sheet.Cells["B4"].PutValue(300);
// Add multiple pivot tables
sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
sheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
sheet.PivotTables.Add("A1:B4", "D20", "PivotTable3");
// Remove pivot table at index 1 (second pivot table)
sheet.PivotTables.RemoveAt(1);
// Verify the count after removal
Console.WriteLine("Pivot Tables Count: " + sheet.PivotTables.Count);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## RemoveAt(int, bool) {#removeat_2}
Deletes the PivotTable at the specified index
```csharp
public void RemoveAt(int index, bool keepData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the position index in PivotTable collection |
| keepData | Boolean | Whether to keep the PivotTable data |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableCollectionMethodRemoveAtWithInt32BooleanDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Demonstrate RemoveAt with keepData=true
worksheet.PivotTables.RemoveAt(0, true);
Console.WriteLine("Pivot table removed with keepData=true. Cell D9 value: " + worksheet.Cells["D9"].Value);
// Add another pivot table
index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable2");
pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Demonstrate RemoveAt with keepData=false
worksheet.PivotTables.RemoveAt(0, false);
Console.WriteLine("Pivot table removed with keepData=false. Cell D9 value: " + worksheet.Cells["D9"].Value);
}
}
}
```
### See Also
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
