##FormatCondition.AboveAverage
FormatCondition property. Get the conditional formattings AboveAverage instance. The default instances rule highlights cells that are above the average for all values in the range. Valid only for type  AboveAverage
## FormatCondition.AboveAverage property
Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage.
```csharp
public AboveAverage AboveAverage { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FormatConditionPropertyAboveAverageDemo
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
worksheet.Cells["A5"].PutValue(50);
// Add above average conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
fcc.AddCondition(FormatConditionType.AboveAverage);
fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });
// Set to highlight above average values
FormatCondition fc = fcc[0];
fc.AboveAverage.IsAboveAverage = true;
fc.Style.BackgroundColor = Color.Yellow;
// Add below average conditional formatting
index = worksheet.ConditionalFormattings.Add();
fcc = worksheet.ConditionalFormattings[index];
fcc.AddCondition(FormatConditionType.AboveAverage);
fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });
// Set to highlight below average values
fc = fcc[0];
fc.AboveAverage.IsAboveAverage = false;
fc.Style.BackgroundColor = Color.LightBlue;
// Save the workbook
workbook.Save("AboveAverageConditionDemo.xlsx");
}
}
}
```
### See Also
* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
