##Class DataBarBorder
Aspose.Cells.DataBarBorder class. Represents the border of the data bars specified by a conditional formatting rule
## DataBarBorder class
Represents the border of the data bars specified by a conditional formatting rule.
```csharp
public class DataBarBorder
```
## Properties
| Name | Description |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | Gets or sets the border's color of data bars specified by a conditional formatting rule. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | Gets or sets the border's type of data bars specified by a conditional formatting rule. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class DataBarBorderDemo
{
public static void DataBarBorderExample()
{
// Creating a new workbook
Workbook workbook = new Workbook();
// Accessing the first worksheet in the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Adding some sample data to the worksheet
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(50);
worksheet.Cells["A3"].PutValue(80);
worksheet.Cells["A4"].PutValue(60);
worksheet.Cells["A5"].PutValue(30);
// Adding an empty conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Defining a cell area for conditional formatting
CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
fcs.AddArea(ca);
// Adding a condition of type DataBar
int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
FormatCondition formatCondition = fcs[conditionIndex];
// Accessing the DataBar
DataBar dataBar = formatCondition.DataBar;
// Setting the DataBar properties
dataBar.Color = Color.Orange;
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
dataBar.MinCfvo.Value = 0;
dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
dataBar.MaxCfvo.Value = 100;
dataBar.ShowValue = true;
// Accessing and setting the DataBarBorder properties
DataBarBorder dataBarBorder = dataBar.BarBorder;
dataBarBorder.Type = DataBarBorderType.Solid;
dataBarBorder.Color = Color.Black;
// Saving the Excel file
workbook.Save("DataBarBorderExample.xlsx");
workbook.Save("DataBarBorderExample.pdf");
Console.WriteLine("DataBar border example created successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
