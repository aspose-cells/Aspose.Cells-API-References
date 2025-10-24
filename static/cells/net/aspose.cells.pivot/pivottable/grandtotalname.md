##PivotTable.GrandTotalName
PivotTable property. Returns the label that is displayed in the grand total column or row heading. The default value is the string Grand Total
## PivotTable.GrandTotalName property
Returns the label that is displayed in the grand total column or row heading. The default value is the string "Grand Total".
```csharp
public string GrandTotalName { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyGrandTotalNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Region";
worksheet.Cells["C1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Laptop";
worksheet.Cells["B2"].Value = "North";
worksheet.Cells["C2"].Value = 1000;
worksheet.Cells["A3"].Value = "Laptop";
worksheet.Cells["B3"].Value = "South";
worksheet.Cells["C3"].Value = 1500;
worksheet.Cells["A4"].Value = "Phone";
worksheet.Cells["B4"].Value = "North";
worksheet.Cells["C4"].Value = 800;
worksheet.Cells["A5"].Value = "Phone";
worksheet.Cells["B5"].Value = "South";
worksheet.Cells["C5"].Value = 1200;
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row and data fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current GrandTotalName value
Console.WriteLine("Current GrandTotalName: " + pivotTable.GrandTotalName);
// Change the GrandTotalName
pivotTable.GrandTotalName = "Total Summary";
// Calculate data and refresh the pivot table
pivotTable.CalculateData();
pivotTable.RefreshData();
// Save the workbook
workbook.Save("PivotTableGrandTotalNameDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
