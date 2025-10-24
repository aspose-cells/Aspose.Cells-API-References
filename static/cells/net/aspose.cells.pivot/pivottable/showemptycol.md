##PivotTable.ShowEmptyCol
PivotTable property. Indicates whether to include empty columns in the table
## PivotTable.ShowEmptyCol property
Indicates whether to include empty columns in the table
```csharp
public bool ShowEmptyCol { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyShowEmptyColDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current value of ShowEmptyCol
Console.WriteLine("Current ShowEmptyCol value: " + pivotTable.ShowEmptyCol);
// Set ShowEmptyCol to false (hide empty columns)
pivotTable.ShowEmptyCol = false;
Console.WriteLine("ShowEmptyCol set to false - empty columns will be hidden");
// Calculate pivot table data
pivotTable.CalculateData();
// Save the workbook with hidden empty columns
workbook.Save("PivotTableHideEmptyCols.xlsx");
// Set ShowEmptyCol back to true (show empty columns)
pivotTable.ShowEmptyCol = true;
Console.WriteLine("ShowEmptyCol set to true - empty columns will be shown");
// Calculate pivot table data again
pivotTable.CalculateData();
// Save the workbook with visible empty columns
workbook.Save("PivotTableShowEmptyCols.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
