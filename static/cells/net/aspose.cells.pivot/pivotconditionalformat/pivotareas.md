##PivotConditionalFormat.PivotAreas
PivotConditionalFormat property. Gets all pivot areas
## PivotConditionalFormat.PivotAreas property
Gets all pivot areas.
```csharp
public PivotAreaCollection PivotAreas { get; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PivotConditionalFormatPropertyPivotAreasDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].Value = "Product";
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["A2"].Value = "Apple";
sheet.Cells["B2"].Value = 150;
sheet.Cells["A3"].Value = "Banana";
sheet.Cells["B3"].Value = 80;
sheet.Cells["A4"].Value = "Orange";
sheet.Cells["B4"].Value = 200;
int pivotIndex = sheet.PivotTables.Add("A5", "A1:B4", "PivotTable");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, 0);
pivot.AddFieldToArea(PivotFieldType.Data, 1);
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
int formatIndex = pivot.ConditionalFormats.Add();
PivotConditionalFormat pcf = pivot.ConditionalFormats[formatIndex];
CellArea cellArea = CellArea.CreateCellArea("B6", "B8");
pcf.AddCellArea(cellArea);
pcf.PivotAreas[0].RuleType = PivotAreaType.Data;
int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition condition = pcf.FormatConditions[conditionIndex];
condition.Operator = OperatorType.GreaterOrEqual;
condition.Formula1 = "100";
condition.Style.BackgroundColor = Color.Red;
pivot.CalculateData();
workbook.Save("PivotAreasDemoOutput.xlsx");
}
}
}
```
### See Also
* class [PivotAreaCollection](../../pivotareacollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
