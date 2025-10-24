##Enum PivotLineType
Aspose.Cells.Pivot.PivotLineType enum. Specifies the type of the PivotLine
## PivotLineType enumeration
Specifies the type of the PivotLine.
```csharp
public enum PivotLineType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Regular | `0` | Regular PivotLine with pivot items. |
| Subtotal | `1` | Subtotal line. |
| GrandTotal | `2` | Grand Total line. |
| Blank | `3` | Blank line after each group. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotClassPivotLineTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(300);
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Sort row field by values in descending order
pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "B2");
// Calculate pivot table data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotLineTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
