##PivotConditionalFormat.FormatConditions
PivotConditionalFormat property. Get conditions for the pivot table conditional format
## PivotConditionalFormat.FormatConditions property
Get conditions for the pivot table conditional format .
```csharp
public FormatConditionCollection FormatConditions { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotConditionalFormatPropertyFormatConditionsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 120;
cells["A3"].Value = "Orange";
cells["B3"].Value = 85;
cells["A4"].Value = "Banana";
cells["B4"].Value = 95;
// Add pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add conditional format
int formatIndex = pivotTable.ConditionalFormats.Add();
PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 1;
area.EndRow = 3;
area.EndColumn = 1;
pfc.AddCellArea(area); // Apply to quantity column
// Add format condition
int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = pfc.FormatConditions[conditionIndex];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = System.Drawing.Color.Red;
// Calculate pivot table data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotConditionalFormatExample.xlsx");
}
}
}
```
### See Also
* class [FormatConditionCollection](../../../aspose.cells/formatconditioncollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
