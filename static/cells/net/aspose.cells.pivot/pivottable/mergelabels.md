##PivotTable.MergeLabels
PivotTable property. True if the specified PivotTable reports outerrow item column item subtotal and grand total labels use merged cells
## PivotTable.MergeLabels property
True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.
```csharp
public bool MergeLabels { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyMergeLabelsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Apple";
worksheet.Cells["A4"].Value = "Orange";
worksheet.Cells["A5"].Value = "Orange";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 8;
worksheet.Cells["B5"].Value = 12;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Enable merging labels
pivotTable.MergeLabels = true;
// Save the workbook
workbook.Save("PivotTableMergeLabelsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
