##Class VerticalPageBreak
Aspose.Cells.VerticalPageBreak class. Encapsulates the object that represents a vertical page break
## VerticalPageBreak class
Encapsulates the object that represents a vertical page break.
```csharp
public class VerticalPageBreak
```
## Properties
| Name | Description |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | Gets the column index of the vertical page break. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | Gets the end row index of the vertical page break. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | Gets the start row index of the vertical page break. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class VerticalPageBreakDemo
{
public static void VerticalPageBreakExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet in the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add a vertical page break at column G (index 6)
worksheet.VerticalPageBreaks.Add("G5");
// Save the workbook
workbook.Save("VerticalPageBreakExample.xlsx");
// Access the added vertical page break
VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
// Display the properties of the vertical page break
Console.WriteLine("Start Row: " + vpb.StartRow);
Console.WriteLine("End Row: " + vpb.EndRow);
Console.WriteLine("Column: " + vpb.Column);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
