##PivotConditionalFormat.RuleType
PivotConditionalFormat property. Get and set rule type for the pivot table condition format
## PivotConditionalFormat.RuleType property
Get and set rule type for the pivot table condition format .
```csharp
public PivotConditionFormatRuleType RuleType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotConditionalFormatPropertyRuleTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create minimal data for pivot table
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "Value";
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:A2", "C3", "DemoPivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add conditional format
int formatIndex = pivotTable.ConditionalFormats.Add();
PivotConditionalFormat format = pivotTable.ConditionalFormats[formatIndex];
// Demonstrate RuleType property
Console.WriteLine("Initial RuleType: " + format.RuleType);
// Set new rule type
format.RuleType = PivotConditionFormatRuleType.Row;
Console.WriteLine("Updated RuleType: " + format.RuleType);
workbook.Save("RuleTypeDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* enum [PivotConditionFormatRuleType](../../pivotconditionformatruletype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
