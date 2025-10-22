##PivotConditionalFormatCollection.Item
PivotConditionalFormatCollection property. Gets the pivot FormatCondition object at the specific index
## PivotConditionalFormatCollection indexer
Gets the pivot FormatCondition object at the specific index.
```csharp
public PivotConditionalFormat this[int index] { get; }
```
### Return Value
pivot FormatCondition object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotConditionalFormatCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
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
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add conditional format
int formatIndex = pivotTable.ConditionalFormats.Add();
PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex]; // Using Item property
pfc.AddCellArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 10, EndColumn = 10 });
// Add format condition
int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition condition = pfc.FormatConditions[conditionIndex];
condition.Formula1 = "90";
condition.Operator = OperatorType.GreaterOrEqual;
condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;
// Calculate pivot table and save
pivotTable.CalculateData();
workbook.Save("PivotConditionalFormatExample.xlsx");
}
}
}
```
### See Also
* class [PivotConditionalFormat](../../pivotconditionalformat/)
* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
