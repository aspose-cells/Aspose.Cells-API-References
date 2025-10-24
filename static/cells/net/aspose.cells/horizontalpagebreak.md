##Class HorizontalPageBreak
Aspose.Cells.HorizontalPageBreak class. Encapsulates the object that represents a horizontal page break
## HorizontalPageBreak class
Encapsulates the object that represents a horizontal page break.
```csharp
public class HorizontalPageBreak
```
## Properties
| Name | Description |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Gets the end column index of this horizontal page break. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Gets the zero based row index. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Gets the start column index of this horizontal page break. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HorizontalPageBreakDemo
{
public static void HorizontalPageBreakExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[0];
// Add a page break at cell Y30
int index = worksheet.HorizontalPageBreaks.Add("Y30");
// Get the newly added horizontal page break
HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
// Display the properties of the horizontal page break
Console.WriteLine("Horizontal Page Break Details:");
Console.WriteLine($"Row: {hPageBreak.Row}");
Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
// Save the workbook
workbook.Save("HorizontalPageBreakExample.xlsx");
workbook.Save("HorizontalPageBreakExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
