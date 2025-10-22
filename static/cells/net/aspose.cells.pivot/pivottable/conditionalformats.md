##PivotTable.ConditionalFormats
PivotTable property. Gets the conditional formats of the pivot table
## PivotTable.ConditionalFormats property
Gets the conditional formats of the pivot table.
```csharp
public PivotConditionalFormatCollection ConditionalFormats { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PivotTablePropertyConditionalFormatsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 120;
cells["A3"].Value = "Orange";
cells["B3"].Value = 85;
cells["A4"].Value = "Banana";
cells["B4"].Value = 95;
cells["A5"].Value = "Apple";
cells["B5"].Value = 110;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row and data fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Add conditional format
int formatIndex = pivotTable.ConditionalFormats.Add();
PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
pcf.AddFieldArea(PivotFieldType.Data, pivotTable.DataFields[0]);
// Add format condition
int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition condition = pcf.FormatConditions[conditionIndex];
condition.Operator = OperatorType.GreaterOrEqual;
condition.Formula1 = "100";
condition.Style.BackgroundColor = Color.Red;
// Save workbook
workbook.Save("PivotTableConditionalFormatting.xlsx");
}
}
}
```
### See Also
* class [PivotConditionalFormatCollection](../../pivotconditionalformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
