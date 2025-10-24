##PivotConditionalFormat.ApplyTo
PivotConditionalFormat method. Applies the conditional format to range. Only for the data region
## PivotConditionalFormat.ApplyTo method
Applies the conditional format to range. Only for the data region.
```csharp
public void ApplyTo(int row, int column, PivotConditionFormatScopeType scope)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The selected row. |
| column | Int32 | The selected column. |
| scope | PivotConditionFormatScopeType | The scope |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotConditionalFormatMethodApplyToWithInt32Int32PivotConditionFormatDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["A5"].PutValue("B");
worksheet.Cells["B5"].PutValue(40);
// Add pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotTableIndex = pivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotTableIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Add conditional format
PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
// Demonstrate ApplyTo method with specific parameters
pcf.ApplyTo(0, 1, PivotConditionFormatScopeType.Field);
// Add format condition
FormatConditionCollection fcc = pcf.FormatConditions;
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "20";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = System.Drawing.Color.LightGreen;
// Calculate data and save
pivotTable.CalculateData();
workbook.Save("PivotConditionalFormatApplyToDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
