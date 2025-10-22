##DataBar.BarFillType
DataBar property. Gets or sets how a data bar is filled with color
## DataBar.BarFillType property
Gets or sets how a data bar is filled with color.
```csharp
public DataBarFillType BarFillType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataBarPropertyBarFillTypeDemo
{
public static void Run()
{
// Instantiate a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Set the conditional format range
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 5,
StartColumn = 0,
EndColumn = 5
};
fcs.AddArea(ca);
// Add DataBar condition
int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
FormatCondition fc = fcs[conditionIndex];
// Configure DataBar properties
DataBar dataBar = fc.DataBar;
dataBar.BarFillType = DataBarFillType.Gradient; // Demonstrating BarFillType usage
dataBar.Color = Color.Blue;
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(50);
worksheet.Cells["A3"].PutValue(100);
// Save the workbook
workbook.Save("DataBarFillTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
