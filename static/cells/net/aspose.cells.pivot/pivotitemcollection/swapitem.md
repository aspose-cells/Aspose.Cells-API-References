##PivotItemCollection.SwapItem
PivotItemCollection method. Directly swap two items
## PivotItemCollection.SwapItem method
Directly swap two items.
```csharp
public void SwapItem(int index1, int index2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index1 | Int32 |  |
| index2 | Int32 |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotItemCollectionMethodSwapItemWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 300;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Get pivot items
PivotField pivotField = pivotTable.RowFields[0];
PivotItemCollection pivotItems = pivotField.PivotItems;
try
{
// Display original order
Console.WriteLine("Original order:");
foreach (PivotItem item in pivotItems)
{
Console.WriteLine(item.Name);
}
// Swap items at index 0 and 1
pivotItems.SwapItem(0, 1);
// Display new order
Console.WriteLine("\nAfter swapping:");
foreach (PivotItem item in pivotItems)
{
Console.WriteLine(item.Name);
}
Console.WriteLine("SwapItem method executed successfully with parameters (0, 1)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SwapItem method: {ex.Message}");
}
// Save the result
workbook.Save("PivotItemCollectionMethodSwapItemWithInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
