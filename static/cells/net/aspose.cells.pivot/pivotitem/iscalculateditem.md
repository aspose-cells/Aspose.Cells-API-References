##PivotItem.IsCalculatedItem
PivotItem property. Indicates whether this pivot item is a calculated formula item
## PivotItem.IsCalculatedItem property
Indicates whether this pivot item is a calculated formula item.
```csharp
public bool IsCalculatedItem { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotItemPropertyIsCalculatedItemDemo
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
worksheet.Cells["A5"].Value = "Apple";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 20;
worksheet.Cells["B4"].Value = 30;
worksheet.Cells["B5"].Value = 15;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Calculate pivot table data
pivotTable.CalculateData();
// Get the first pivot item from the first pivot field
PivotField pivotField = pivotTable.RowFields[0];
PivotItem pivotItem = pivotField.PivotItems[0];
// Display the IsCalculatedItem property value
Console.WriteLine("IsCalculatedItem value: " + pivotItem.IsCalculatedItem);
// Check if the pivot item is a calculated item
if (pivotItem.IsCalculatedItem)
{
Console.WriteLine("This pivot item is a calculated formula item.");
Console.WriteLine("Formula: " + pivotItem.GetFormula());
}
else
{
Console.WriteLine("This pivot item is not a calculated formula item.");
}
// Save the workbook
workbook.Save("PivotItemPropertyIsCalculatedItemDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
