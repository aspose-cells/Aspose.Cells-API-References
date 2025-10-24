##PivotItem.Position
PivotItem property. Specifying the position index in all the PivotItemsnot the PivotItems under the same parent node
## PivotItem.Position property
Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.
```csharp
public int Position { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemPropertyPositionDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Banana");
sheet.Cells["A4"].PutValue("Orange");
sheet.Cells["B2"].PutValue(1000);
sheet.Cells["B3"].PutValue(2000);
sheet.Cells["B4"].PutValue(3000);
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Demonstrate Position property
PivotField rowField = pivotTable.RowFields[0];
foreach (PivotItem item in rowField.PivotItems)
{
Console.WriteLine($"Before - Name: {item.Name}, Position: {item.Position}");
item.Position = 0; // Set position to 0
Console.WriteLine($"After - Name: {item.Name}, Position: {item.Position}");
}
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotItemPositionDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
