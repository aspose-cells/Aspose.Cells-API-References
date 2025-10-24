##DataBar.Direction
DataBar property. Gets or sets the direction the databar is displayed
## DataBar.Direction property
Gets or sets the direction the databar is displayed.
```csharp
public TextDirectionType Direction { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DataBarPropertyDirectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to demonstrate data bars
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
}
// Add data bar conditional formatting
ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
int index = conditionalFormattings.Add();
FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
// Define the cell area for the format condition
CellArea cellArea = new CellArea
{
StartRow = 0,
StartColumn = 0,
EndRow = 9,
EndColumn = 0
};
conditionalFormatting.AddArea(cellArea);
// Add the DataBar condition and get reference
int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
FormatCondition condition = conditionalFormatting[conditionIndex];
DataBar dataBar = condition.DataBar;
// Display current Direction value
Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);
// Change direction to RightToLeft and demonstrate
dataBar.Direction = TextDirectionType.RightToLeft;
// Additional configuration for better visualization
dataBar.Color = System.Drawing.Color.LightGreen;
dataBar.MinCfvo.Type = FormatConditionValueType.Min;
dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
// Save the workbook to show the effect
workbook.Save("DataBarDirectionDemo.xlsx");
}
}
}
```
### See Also
* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
