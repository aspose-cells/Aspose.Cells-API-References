##PivotTable.GetFields
PivotTable method. Gets the specific pivot field list by the region
## PivotTable.GetFields method
Gets the specific pivot field list by the region.
```csharp
public PivotFieldCollection GetFields(PivotFieldType fieldType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the region type. |
### Return Value
the specific pivot field collection
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableMethodGetFieldsWithPivotFieldTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 20;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
try
{
// Call GetFields method with PivotFieldType.Row parameter
PivotFieldCollection rowFields = pivotTable.GetFields(PivotFieldType.Row);
Console.WriteLine($"Number of row fields: {rowFields.Count}");
foreach (PivotField field in rowFields)
{
Console.WriteLine($"Row field name: {field.Name}");
}
// Call GetFields method with PivotFieldType.Data parameter
PivotFieldCollection dataFields = pivotTable.GetFields(PivotFieldType.Data);
Console.WriteLine($"Number of data fields: {dataFields.Count}");
foreach (PivotField field in dataFields)
{
Console.WriteLine($"Data field name: {field.Name}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFields method: {ex.Message}");
}
// Save the workbook
workbook.Save("PivotTableGetFieldsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
