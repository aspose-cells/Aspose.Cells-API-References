##PivotTable.ShowEmptyRow
PivotTable property. Indicates whether to include empty rows in the table
## PivotTable.ShowEmptyRow property
Indicates whether to include empty rows in the table.
```csharp
public bool ShowEmptyRow { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyShowEmptyRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with some empty rows
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["B1"].Value = "Product";
worksheet.Cells["C1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Electronics";
worksheet.Cells["B2"].Value = "TV";
worksheet.Cells["C2"].Value = 1000;
worksheet.Cells["A3"].Value = "Electronics";
worksheet.Cells["B3"].Value = "";
worksheet.Cells["C3"].Value = "";
worksheet.Cells["A4"].Value = "Furniture";
worksheet.Cells["B4"].Value = "Chair";
worksheet.Cells["C4"].Value = 500;
worksheet.Cells["A5"].Value = "Furniture";
worksheet.Cells["B5"].Value = "";
worksheet.Cells["C5"].Value = "";
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display current ShowEmptyRow value
Console.WriteLine("Initial ShowEmptyRow value: " + pivotTable.ShowEmptyRow);
// Show empty rows in the pivot table
pivotTable.ShowEmptyRow = true;
Console.WriteLine("ShowEmptyRow set to: " + pivotTable.ShowEmptyRow);
// Calculate data to populate the pivot table
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableShowEmptyRowDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
