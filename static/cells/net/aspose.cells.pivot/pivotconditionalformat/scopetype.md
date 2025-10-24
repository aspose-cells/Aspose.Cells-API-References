##PivotConditionalFormat.ScopeType
PivotConditionalFormat property. Get and set scope type for the pivot table conditional format
## PivotConditionalFormat.ScopeType property
Get and set scope type for the pivot table conditional format .
```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PivotConditionalFormatPropertyScopeTypeDemo
{
public static void Run()
{
// Create a workbook with a pivot table
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Sample data for pivot table
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["B2"].PutValue(100);
sheet.Cells["A3"].PutValue("B");
sheet.Cells["B3"].PutValue(200);
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B4"].PutValue(300);
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add conditional format to pivot table
int formatIndex = pivotTable.ConditionalFormats.Add();
PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
pcf.ScopeType = PivotConditionFormatScopeType.Data;
// Add format condition
FormatConditionCollection fcs = pcf.FormatConditions;
CellArea area = new CellArea();
area.StartRow = 4;
area.EndRow = 6;
area.StartColumn = 5;
area.EndColumn = 5;
int[] conditionIndex = fcs.Add(area, FormatConditionType.CellValue, OperatorType.Between, "100", "200");
// Set format style
FormatCondition fc = fcs[conditionIndex[0]];
fc.Style.BackgroundColor = Color.Yellow;
// Save the workbook
wb.Save("PivotConditionalFormatScopeTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
