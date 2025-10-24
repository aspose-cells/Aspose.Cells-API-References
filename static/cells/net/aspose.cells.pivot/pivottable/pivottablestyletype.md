##PivotTable.PivotTableStyleType
PivotTable property. Gets and sets the builtin pivot table style
## PivotTable.PivotTableStyleType property
Gets and sets the built-in pivot table style.
```csharp
public PivotTableStyleType PivotTableStyleType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyPivotTableStyleTypeDemo
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
cells["B3"].Value = 5;
cells["A4"].Value = "Banana";
cells["B4"].Value = 7;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Set and demonstrate PivotTableStyleType
pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
Console.WriteLine("PivotTable Style Type: " + pivotTable.PivotTableStyleType);
// Save the workbook
workbook.Save("PivotTableStyleTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
