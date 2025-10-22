##PivotTable.ShowPivotStyleColumnStripes
PivotTable property. Indicates whether stripe formatting is applied for column
## PivotTable.ShowPivotStyleColumnStripes property
Indicates whether stripe formatting is applied for column.
```csharp
public bool ShowPivotStyleColumnStripes { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowPivotStyleColumnStripesDemo
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
cells["A5"].Value = "Apple";
cells["B5"].Value = 5;
cells["A6"].Value = "Orange";
cells["B6"].Value = 12;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity
// Enable column stripes
pivotTable.ShowPivotStyleColumnStripes = true;
// Save the workbook
workbook.Save("PivotTableColumnStripesDemo.xlsx");
Console.WriteLine("Pivot table with column stripes created successfully.");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
