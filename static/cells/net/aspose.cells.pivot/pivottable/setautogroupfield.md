##PivotTable.SetAutoGroupField
PivotTable method. Sets auto field group by the PivotTable
## SetAutoGroupField(int) {#setautogroupfield_1}
Sets auto field group by the PivotTable.
```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetAutoGroupField(int baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The row or column field index in the base fields |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableMethodSetAutoGroupFieldWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["A5"].PutValue("Grape");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
worksheet.Cells["B5"].PutValue(4000);
// Add a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
try
{
// Call SetAutoGroupField with baseFieldIndex parameter (Int32)
// Note: This method is marked as obsolete in the API
pivotTable.SetAutoGroupField(0);
Console.WriteLine("SetAutoGroupField method executed successfully with parameter (Int32)");
// Calculate data to show the effect
pivotTable.CalculateData();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetAutoGroupField method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableMethodSetAutoGroupFieldWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## SetAutoGroupField(PivotField) {#setautogroupfield}
Sets auto field group by the PivotTable.
```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetAutoGroupField(PivotField pivotField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the specific fields |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableMethodSetAutoGroupFieldWithPivotFieldDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["A5"].PutValue("Grapes");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(5);
worksheet.Cells["B4"].PutValue(8);
worksheet.Cells["B5"].PutValue(12);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
// Get the pivot field to group
PivotField pivotField = pivotTable.RowFields[0];
try
{
// Call the SetAutoGroupField method with PivotField parameter
pivotTable.SetAutoGroupField(pivotField);
// Calculate data to update pivot table
pivotTable.CalculateData();
Console.WriteLine("SetAutoGroupField method executed successfully with PivotField parameter");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetAutoGroupField method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableMethodSetAutoGroupFieldWithPivotFieldDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
