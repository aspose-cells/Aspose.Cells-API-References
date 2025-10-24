##DataBar.ShowValue
DataBar property. Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true
## DataBar.ShowValue property
Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true.
```csharp
public bool ShowValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataBarPropertyShowValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].PutValue(30);
sheet.Cells["A4"].PutValue(40);
// Add data bar conditional formatting
int idx = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 3;
area.StartColumn = 0;
area.EndColumn = 0;
fcc.AddArea(area);
// Add data bar condition
int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
FormatCondition fc = fcc[conditionIndex];
// Set data bar properties
fc.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
fc.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
fc.DataBar.Color = Color.Green;
// Demonstrate ShowValue property
fc.DataBar.ShowValue = true; // Show cell values along with data bars
// Save the workbook
workbook.Save("DataBarShowValueDemo.xlsx");
Console.WriteLine("DataBar ShowValue demo completed. Output file: DataBarShowValueDemo.xlsx");
}
}
}
```
### See Also
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
