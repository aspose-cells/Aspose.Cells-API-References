##PivotTable.DisplayImmediateItems
PivotTable property. Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true
## PivotTable.DisplayImmediateItems property
Indicates whether items in the row and column areas are visible when the data area of the PivotTable is empty. The default value is true.
```csharp
public bool DisplayImmediateItems { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyDisplayImmediateItemsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 20;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Demonstrate DisplayImmediateItems property
Console.WriteLine("Initial DisplayImmediateItems value: " + pivotTable.DisplayImmediateItems);
// Change the property value
pivotTable.DisplayImmediateItems = false;
Console.WriteLine("After setting to false: " + pivotTable.DisplayImmediateItems);
// Save the workbook
workbook.Save("PivotTableDisplayImmediateItemsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
