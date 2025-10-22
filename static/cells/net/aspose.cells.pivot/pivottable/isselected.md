##PivotTable.IsSelected
PivotTable property. Indicates whether this PivotTable is selected
## PivotTable.IsSelected property
Indicates whether this PivotTable is selected.
```csharp
public bool IsSelected { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PivotTablePropertyIsSelectedDemo
{
public static void Run()
{
// Create a new workbook
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
// Add a pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
// Initially, IsSelected is false
Console.WriteLine("PivotTable IsSelected initially: " + pivotTable.IsSelected);
// Select the pivot table
pivotTable.IsSelected = true;
Console.WriteLine("PivotTable IsSelected after setting to true: " + pivotTable.IsSelected);
// Deselect the pivot table
pivotTable.IsSelected = false;
Console.WriteLine("PivotTable IsSelected after setting to false: " + pivotTable.IsSelected);
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
