##PivotTable.ShowValuesRow
PivotTable property. Indicates whether showing values row
## PivotTable.ShowValuesRow property
Indicates whether showing values row.
```csharp
public bool ShowValuesRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowValuesRowDemo
{
public static void Run()
{
// Create a workbook with sample data
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
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as row
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity as data
// Demonstrate ShowValuesRow property
Console.WriteLine("Initial ShowValuesRow: " + pivotTable.ShowValuesRow);
pivotTable.ShowValuesRow = true;
Console.WriteLine("After setting to true: " + pivotTable.ShowValuesRow);
// Save the workbook
workbook.Save("PivotTableShowValuesRowDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
