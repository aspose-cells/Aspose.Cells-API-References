##DataBar.MaxLength
DataBar property. Represents the max length of data bar
## DataBar.MaxLength property
Represents the max length of data bar .
```csharp
public int MaxLength { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataBarPropertyMaxLengthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Add conditional formatting
int formatIndex = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
CellArea area = new CellArea
{
StartRow = 0,
EndRow = 3,
StartColumn = 0,
EndColumn = 0
};
fcc.AddArea(area);
// Add data bar and set properties
int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
DataBar dataBar = fcc[conditionIndex].DataBar;
dataBar.Color = Color.Blue;
dataBar.MinLength = 0;
dataBar.MaxLength = 90; // Demonstrating MaxLength property
workbook.Save("DataBarMaxLengthDemo.xlsx");
}
}
}
```
### See Also
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
