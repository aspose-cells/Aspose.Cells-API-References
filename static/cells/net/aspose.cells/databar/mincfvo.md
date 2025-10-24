##DataBar.MinCfvo
DataBar property. Get or set this DataBars min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it
## DataBar.MinCfvo property
Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.
```csharp
public ConditionalFormattingValue MinCfvo { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataBarPropertyMinCfvoDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Get the conditional formatting collection
ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
int index = cfc.Add();
FormatConditionCollection fcc = cfc[index];
// Create a data bar with MinCfvo set to "Value" type
fcc.AddCondition(FormatConditionType.DataBar);
DataBar dataBar = fcc[0].DataBar;
dataBar.MinCfvo.Type = FormatConditionValueType.Min;
dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar
// Set the data bar range
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 3;
area.EndColumn = 0;
fcc.AddArea(area);
// Save the workbook
workbook.Save("DataBarMinCfvoDemo.xlsx");
}
}
}
```
### See Also
* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
