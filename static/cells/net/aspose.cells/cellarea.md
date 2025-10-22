##Struct CellArea
Aspose.Cells.CellArea struct. Represent an area of cells
## CellArea structure
Represent an area of cells.
```csharp
public struct CellArea : IComparable
```
## Methods
| Name | Description |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Creates a cell area. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Creates a cell area. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | Compare two CellArea objects according to their top-left corner. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Returns a string represents the current cell area object. |
## Fields
| Name | Description |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Gets or set the end column of this area. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Gets or set the end row of this area. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Gets or set the start column of this area. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Gets or set the start row of this area. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellAreaDemo
{
public static void CellAreaExample()
{
// Create a new Workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["B2"].PutValue(4);
worksheet.Cells["B5"].PutValue(20);
worksheet.Cells["B8"].PutValue(50);
worksheet.Cells["C2"].PutValue(8);
worksheet.Cells["C7"].PutValue(15);
worksheet.Cells["C9"].PutValue(30);
// Create Cell Area
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 10;
ca.StartColumn = 0;
ca.EndColumn = 10;
// Add a conditional formatting rule to the worksheet
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
fcs.AddArea(ca);
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = System.Drawing.Color.Yellow;
// Save the workbook
workbook.Save("CellAreaExample.xlsx");
workbook.Save("CellAreaExample.pdf");
// Demonstrate the ToString method
Console.WriteLine(ca.ToString());
// Demonstrate the CompareTo method
CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
int comparisonResult = ca.CompareTo(ca2);
Console.WriteLine($"Comparison result: {comparisonResult}");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
