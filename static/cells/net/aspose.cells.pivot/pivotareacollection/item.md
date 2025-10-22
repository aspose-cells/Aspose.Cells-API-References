##PivotAreaCollection.Item
PivotAreaCollection property. Gets a PivotArea object
## PivotAreaCollection indexer
Gets a [`PivotArea`](../../pivotarea/) object;
```csharp
public PivotArea this[int index] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PivotAreaCollectionPropertyItemDemo
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
cells["B2"].Value = 100;
cells["A3"].Value = "Orange";
cells["B3"].Value = 150;
cells["A4"].Value = "Banana";
cells["B4"].Value = 200;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int pivotIndex = pivotTables.Add("A5", "A1:B4", "PivotTable");
PivotTable pivot = pivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, 0);
pivot.AddFieldToArea(PivotFieldType.Data, 1);
// Add conditional format
int formatIndex = pivot.ConditionalFormats.Add();
PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
pfc.AddCellArea(CellArea.CreateCellArea("A5", "B8"));
// Access PivotAreas using Item property
PivotArea pivotArea = pfc.PivotAreas[0]; // Using Item indexer
pivotArea.RuleType = PivotAreaType.All;
// Add format condition
int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition condition = pfc.FormatConditions[conditionIndex];
condition.Formula1 = "150";
condition.Operator = OperatorType.GreaterOrEqual;
condition.Style.BackgroundColor = Color.Red;
// Calculate and save
pivot.CalculateData();
workbook.Save("PivotAreaCollectionPropertyItemDemo_output.xlsx");
}
}
}
```
### See Also
* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
