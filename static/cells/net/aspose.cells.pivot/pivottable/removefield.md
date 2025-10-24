##PivotTable.RemoveField
PivotTable method. Removes a field from specific field area
## RemoveField(PivotFieldType, string) {#removefield_2}
Removes a field from specific field area
```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| fieldName | String | The name in the base fields. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the first pivot table
PivotTable pivotTable = worksheet.PivotTables[0];
// Remove field "c" from Data area
pivotTable.RemoveField(PivotFieldType.Data, "c");
// Calculate pivot table data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## RemoveField(PivotFieldType, int) {#removefield_1}
Removes a field from specific field area
```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| baseFieldIndex | Int32 | The field index in the base fields. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
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
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
try
{
// Remove the row field (index 0) from the pivot table
pivotTable.RemoveField(PivotFieldType.Row, 0);
Console.WriteLine("Row field removed successfully from the pivot table");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableRemoveFieldDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## RemoveField(PivotFieldType, PivotField) {#removefield}
Remove field from specific field area
```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the fields area type. |
| pivotField | PivotField | the field in the base fields. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("TestFile.xlsx");
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the first pivot table
PivotTable pivotTable = worksheet.PivotTables[0];
// Remove a column field from the pivot table
if (pivotTable.ColumnFields.Count > 0)
{
pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
}
// Remove a data field from the pivot table
if (pivotTable.DataFields.Count > 0)
{
pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
}
// Save the workbook
workbook.Save("ModifiedPivotTable.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
