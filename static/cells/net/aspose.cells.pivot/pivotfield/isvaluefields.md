##PivotField.IsValueFields
PivotField property. Indicates whether this field represents values fields
## PivotField.IsValueFields property
Indicates whether this field represents values fields.
```csharp
public bool IsValueFields { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldPropertyIsValueFieldsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Region";
worksheet.Cells["C1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Bike";
worksheet.Cells["A3"].Value = "Bike";
worksheet.Cells["A4"].Value = "Car";
worksheet.Cells["A5"].Value = "Car";
worksheet.Cells["B2"].Value = "East";
worksheet.Cells["B3"].Value = "West";
worksheet.Cells["B4"].Value = "East";
worksheet.Cells["B5"].Value = "West";
worksheet.Cells["C2"].Value = 1000;
worksheet.Cells["C3"].Value = 2000;
worksheet.Cells["C4"].Value = 3000;
worksheet.Cells["C5"].Value = 4000;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add column field
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
// Add data field and get it from DataFields collection
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField dataField = pivotTable.DataFields[0];
// Display the IsValueFields property value
Console.WriteLine("IsValueFields for data field: " + dataField.IsValueFields);
// Try to find a non-data field to show IsValueFields is false
foreach (PivotField field in pivotTable.RowFields)
{
Console.WriteLine("IsValueFields for row field '" + field.Name + "': " + field.IsValueFields);
}
// Save the result
workbook.Save("PivotFieldPropertyIsValueFieldsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
