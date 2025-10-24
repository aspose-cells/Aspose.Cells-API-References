##PivotField.InitPivotItems
PivotField method. Init the pivot items of the pivot field
## PivotField.InitPivotItems method
Init the pivot items of the pivot field
```csharp
public void InitPivotItems()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldMethodInitPivotItemsDemo
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
worksheet.Cells["A3"].PutValue("Car");
worksheet.Cells["A4"].PutValue("Bike");
worksheet.Cells["A5"].PutValue("Car");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(1500);
worksheet.Cells["B5"].PutValue(2500);
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields[0];
try
{
// Initialize pivot items
pivotField.InitPivotItems();
// Display the pivot items
Console.WriteLine("Pivot Items after initialization:");
foreach (PivotItem item in pivotField.PivotItems)
{
Console.WriteLine(item.Name);
}
// Save the workbook
workbook.Save("PivotFieldInitPivotItemsDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing InitPivotItems method: {ex.Message}");
}
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
