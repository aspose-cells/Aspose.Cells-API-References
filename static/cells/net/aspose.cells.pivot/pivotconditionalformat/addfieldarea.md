##PivotConditionalFormat.AddFieldArea
PivotConditionalFormat method. Adds an area of pivot field
## AddFieldArea(PivotFieldType, string) {#addfieldarea_1}
Adds an area of pivot field.
```csharp
public void AddFieldArea(PivotFieldType axisType, string fieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region type. |
| fieldName | String | The name of pivot field. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PivotConditionalFormatMethodAddFieldAreaWithPivotFieldTypeStringDemo
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
// Create pivot table - fixed by getting the pivot table from the index
int pivotTableIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Add conditional format
PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
pcf.ScopeType = PivotConditionFormatScopeType.Field;
// Demonstrate AddFieldArea with PivotFieldType and string parameters
pcf.AddFieldArea(PivotFieldType.Data, "Value");
pcf.AddFieldArea(PivotFieldType.Row, "Category");
// Add format condition
FormatConditionCollection fcc = pcf.FormatConditions;
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "20";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundArgbColor = Color.LightGreen.ToArgb();
// Calculate data and save
pivotTable.RefreshData();
pivotTable.CalculateData();
workbook.Save("PivotConditionalFormatDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## AddFieldArea(PivotFieldType, PivotField) {#addfieldarea}
Adds an area of pivot field.
```csharp
public void AddFieldArea(PivotFieldType axisType, PivotField field)
```
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region type. |
| field | PivotField | The pivot field. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotConditionalFormatMethodAddFieldAreaWithPivotFieldTypePivotFieldDemo
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
cells["A3"].Value = "Orange";
cells["A4"].Value = "Banana";
cells["B2"].Value = 100;
cells["B3"].Value = 150;
cells["B4"].Value = 200;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A5", "A1:B4", "PivotTable");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add fields to pivot areas
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // First field (Fruit) as row
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Second field (Quantity) as data
// Add conditional format
int formatIndex = pivotTable.ConditionalFormats.Add();
PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
// Demonstrate AddFieldArea with PivotFieldType and PivotField parameters
pfc.AddFieldArea(PivotFieldType.Row, pivotTable.RowFields[0]);
// Add format condition
int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition condition = pfc.FormatConditions[conditionIndex];
condition.Formula1 = "100";
condition.Operator = OperatorType.GreaterOrEqual;
condition.Style.BackgroundColor = System.Drawing.Color.Red;
// Save the workbook
workbook.Save("PivotConditionalFormatExample.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
