##VerticalPageBreak.EndRow
VerticalPageBreak property. Gets the end row index of the vertical page break
## VerticalPageBreak.EndRow property
Gets the end row index of the vertical page break.
```csharp
public int EndRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakPropertyEndRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a vertical page break that spans rows 3 to 8 at column C (index 2)
worksheet.VerticalPageBreaks.Add("C3:C8");
// Get the first vertical page break
VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
// Display the end row of the page break
Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
// Since EndRow is read-only, we'll demonstrate getting it but not setting it
// The following line is removed as it causes compilation error:
// vpb.EndRow = 10;
// Instead, we'll add another page break with different end row
worksheet.VerticalPageBreaks.Add("C3:C10");
VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
}
}
}
```
### See Also
* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
