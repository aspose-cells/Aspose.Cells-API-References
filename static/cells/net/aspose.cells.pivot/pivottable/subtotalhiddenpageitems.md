##PivotTable.SubtotalHiddenPageItems
PivotTable property. Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals block totals and grand totals. The default value is False
## PivotTable.SubtotalHiddenPageItems property
Indicates whether hidden page field items in the PivotTable report are included in row and column subtotals, block totals, and grand totals. The default value is False.
```csharp
public bool SubtotalHiddenPageItems { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertySubtotalHiddenPageItemsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Region";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Apple";
cells["B2"].Value = "North";
cells["C2"].Value = 1000;
cells["A3"].Value = "Orange";
cells["B3"].Value = "South";
cells["C3"].Value = 2000;
cells["A4"].Value = "Banana";
cells["B4"].Value = "North";
cells["C4"].Value = 1500;
cells["A5"].Value = "Apple";
cells["B5"].Value = "South";
cells["C5"].Value = 1200;
// Create pivot table
int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Set SubtotalHiddenPageItems property
pivotTable.SubtotalHiddenPageItems = true;
Console.WriteLine("SubtotalHiddenPageItems set to: " + pivotTable.SubtotalHiddenPageItems);
// Refresh and calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTable_SubtotalHiddenPageItemsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
