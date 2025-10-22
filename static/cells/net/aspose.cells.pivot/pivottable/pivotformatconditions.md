##PivotTable.PivotFormatConditions
PivotTable property. Gets the Format Conditions of the pivot table
## PivotTable.PivotFormatConditions property
Gets the Format Conditions of the pivot table.
```csharp
[Obsolete("Use PivotTable.ConditionalFormats property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFormatConditionCollection PivotFormatConditions { get; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotTable.ConditionalFormats property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PivotTablePropertyPivotFormatConditionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].Value = "Product";
cells["B1"].Value = "Year";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Laptop";
cells["A3"].Value = "Phone";
cells["A4"].Value = "Tablet";
cells["A5"].Value = "Laptop";
cells["A6"].Value = "Phone";
cells["A7"].Value = "Tablet";
cells["B2"].Value = 2020;
cells["B3"].Value = 2020;
cells["B4"].Value = 2020;
cells["B5"].Value = 2021;
cells["B6"].Value = 2021;
cells["B7"].Value = 2021;
cells["C2"].Value = 1500;
cells["C3"].Value = 800;
cells["C4"].Value = 400;
cells["C5"].Value = 1800;
cells["C6"].Value = 950;
cells["C7"].Value = 500;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:C7", "E3", "SalesPivot");
PivotTable pivot = worksheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Product");
pivot.AddFieldToArea(PivotFieldType.Column, "Year");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
// Add format condition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition condition = fcc[conditionIndex];
condition.Formula1 = "1000";
condition.Operator = OperatorType.GreaterOrEqual;
condition.Style.BackgroundColor = Color.LightGreen;
pfc.ScopeType = PivotConditionFormatScopeType.Data;
// Refresh and save
pivot.RefreshData();
workbook.Save("PivotTableFormatConditionsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFormatConditionCollection](../../pivotformatconditioncollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
