##PivotField.PivotItems
PivotField property. Gets the pivot items of the pivot field
## PivotField.PivotItems property
Gets the pivot items of the pivot field
```csharp
public PivotItemCollection PivotItems { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyPivotItemsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["B1"].Value = "Value";
worksheet.Cells["A2"].Value = "A";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["A3"].Value = "B";
worksheet.Cells["B3"].Value = 20;
worksheet.Cells["A4"].Value = "A";
worksheet.Cells["B4"].Value = 30;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Refresh data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Get the pivot field and demonstrate PivotItems
PivotField field = pivotTable.RowFields[0];
Console.WriteLine("Field Name: " + field.Name);
Console.WriteLine("Total PivotItems: " + field.PivotItems.Count);
// Display all pivot item names
foreach (PivotItem item in field.PivotItems)
{
Console.WriteLine("Item Name: " + item.Name);
}
}
}
}
```
### See Also
* class [PivotItemCollection](../../pivotitemcollection/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
