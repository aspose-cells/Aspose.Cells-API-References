##DataBar.MinLength
DataBar property. Represents the min length of data bar
## DataBar.MinLength property
Represents the min length of data bar .
```csharp
public int MinLength { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DataBarPropertyMinLengthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["A2"].PutValue(15);
worksheet.Cells["A3"].PutValue(25);
worksheet.Cells["A4"].PutValue(35);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 3,
StartColumn = 0,
EndColumn = 0
};
fcc.AddArea(ca);
// Add data bar
int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
FormatCondition fc = fcc[conditionIndex];
DataBar dataBar = fc.DataBar;
// Configure data bar
dataBar.Color = Color.Green;
dataBar.MinLength = 10;  // Minimum length set to 10%
dataBar.MaxLength = 100;
workbook.Save("DataBarMinLengthDemo.xlsx");
Console.WriteLine("DataBar with MinLength demo executed successfully.");
}
}
}
```
### See Also
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
