##PivotTable.RowGrand
PivotTable property. Indicates whether to show grand totals for rows of this pivot table
## PivotTable.RowGrand property
Indicates whether to show grand totals for rows of this pivot table.
```csharp
[Obsolete("Use PivotTable.ShowRowGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool RowGrand { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotTable.ShowRowGrandTotals method. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyRowGrandDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Region");
worksheet.Cells["C1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["B2"].PutValue("North");
worksheet.Cells["C2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B3"].PutValue("South");
worksheet.Cells["C3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Product C");
worksheet.Cells["B4"].PutValue("East");
worksheet.Cells["C4"].PutValue(3000);
worksheet.Cells["A5"].PutValue("Product A");
worksheet.Cells["B5"].PutValue("West");
worksheet.Cells["C5"].PutValue(1500);
worksheet.Cells["A6"].PutValue("Product B");
worksheet.Cells["B6"].PutValue("North");
worksheet.Cells["C6"].PutValue(2500);
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:C6", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current value of RowGrand
Console.WriteLine("Current RowGrand value: " + pivotTable.RowGrand);
// Change the RowGrand property
pivotTable.RowGrand = false;
// Calculate pivot table data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTablePropertyRowGrandDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
