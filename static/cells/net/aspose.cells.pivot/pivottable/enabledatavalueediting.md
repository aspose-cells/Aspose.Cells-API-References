##PivotTable.EnableDataValueEditing
PivotTable property. Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area
## PivotTable.EnableDataValueEditing property
Specifies a boolean value that indicates whether the user is allowed to edit the cells in the data area of the pivottable. Enable cell editing in the values area
```csharp
public bool EnableDataValueEditing { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyEnableDataValueEditingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Bike");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Car");
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Bike");
worksheet.Cells["B4"].PutValue(1500);
worksheet.Cells["A5"].PutValue("Car");
worksheet.Cells["B5"].PutValue(3000);
// Add a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current value of EnableDataValueEditing
Console.WriteLine("Current EnableDataValueEditing value: " + pivotTable.EnableDataValueEditing);
// Enable editing of data values
pivotTable.EnableDataValueEditing = true;
// Calculate data to populate the pivot table
pivotTable.CalculateData();
// Save the workbook before editing
workbook.Save("PivotTableBeforeEdit.xlsx");
// Now we can edit the data values directly in the pivot table
// For demonstration, we'll modify a cell in the data area
Cell dataCell = worksheet.Cells["F5"]; // Assuming this is a data cell
if (dataCell != null)
{
dataCell.PutValue(2500); // Modify the value
}
// Save the workbook after editing
workbook.Save("PivotTableAfterEdit.xlsx");
// Disable editing of data values
pivotTable.EnableDataValueEditing = false;
Console.WriteLine("EnableDataValueEditing set to: " + pivotTable.EnableDataValueEditing);
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
