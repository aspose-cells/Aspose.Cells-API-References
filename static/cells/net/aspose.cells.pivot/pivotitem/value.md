##PivotItem.Value
PivotItem property. Gets the value of the pivot item
## PivotItem.Value property
Gets the value of the pivot item
```csharp
public object Value { get; }
```
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemPropertyValueDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 20;
cells["A5"].Value = "Apple";
cells["B5"].Value = 5;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields[0];
// Process pivot items
List<string> valuesToShow = new List<string> { "Apple", "Banana" };
Console.WriteLine("Pivot Items Before Filtering:");
PrintPivotItems(pivotField);
// Filter pivot items based on Value property
for (int i = 0; i < pivotField.PivotItems.Count; i++)
{
PivotItem item = pivotField.PivotItems[i];
string itemValue = item.Value?.ToString() ?? "";
if (!valuesToShow.Contains(itemValue))
{
item.IsHidden = true;
}
}
Console.WriteLine("\nPivot Items After Filtering:");
PrintPivotItems(pivotField);
}
private static void PrintPivotItems(PivotField pivotField)
{
for (int i = 0; i < pivotField.PivotItems.Count; i++)
{
PivotItem item = pivotField.PivotItems[i];
Console.WriteLine($"Name: {item.Name}, Value: {item.Value}, Hidden: {item.IsHidden}");
}
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
