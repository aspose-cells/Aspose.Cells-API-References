##Class AboveAverage
Aspose.Cells.AboveAverage class. Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range
## AboveAverage class
Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.
```csharp
public class AboveAverage
```
## Constructors
| Name | Description |
| --- | --- |
| [AboveAverage](aboveaverage/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class AboveAverageDemo
{
public static void AboveAverageExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a conditional formatting collection to the worksheet
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Define the cell area to apply the conditional formatting
CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
fcs.AddArea(ca);
// Add an above average condition to the collection
int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
FormatCondition fc = fcs[conditionIndex];
// Set the background color for the condition
fc.Style.BackgroundColor = Color.Yellow;
// Set properties for the above average condition
fc.AboveAverage.IsAboveAverage = true;
fc.AboveAverage.IsEqualAverage = false;
fc.AboveAverage.StdDev = 2;
Cells cells = worksheet.Cells;
cells["A1"].Value = 20;
cells["A2"].Value = 300;
cells["A3"].Value = 40;
cells["A4"].Value = 500;
cells["A5"].Value = 6;
cells["A6"].Value = 70;
cells["A7"].Value = 8;
cells["A8"].Value = 900;
cells["A9"].Value = 10;
cells["C1"].Value = 2;
cells["C2"].Value = 3;
cells["C3"].Value = 4;
cells["C4"].Value = 5;
cells["C5"].Value = 3;
cells["C6"].Value = 2;
cells["C7"].Value = 8;
cells["C8"].Value = 300;
cells["C9"].Value = 10;
// Save the workbook
workbook.Save("AboveAverageExample.xlsx");
workbook.Save("AboveAverageExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
