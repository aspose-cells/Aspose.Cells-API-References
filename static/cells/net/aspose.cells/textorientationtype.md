##Enum TextOrientationType
Aspose.Cells.TextOrientationType enum. Enumerates text orientation types
## TextOrientationType enumeration
Enumerates text orientation types.
```csharp
public enum TextOrientationType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| ClockWise | `0` | Rotates text with 90 degrees clockwise. |
| CounterClockWise | `1` | Rotates text with 90 degrees counterclockwise. |
| NoRotation | `2` | Represents the default value. |
| TopToBottom | `3` | Displays text from top to bottom of the cell. Stacked text. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class TextOrientationTypeDemo
{
public static void TextOrientationTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Hello, Aspose!");
worksheet.Cells["A2"].PutValue("This is a test comment.");
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add(0, 0);
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a comment with text orientation.";
// Set different text orientation types for the comment
comment.TextOrientationType = TextOrientationType.ClockWise;
Console.WriteLine("Text Orientation: ClockWise");
// Save the workbook
workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");
// Change text orientation to CounterClockWise
comment.TextOrientationType = TextOrientationType.CounterClockWise;
Console.WriteLine("Text Orientation: CounterClockWise");
// Save the workbook
workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");
// Change text orientation to NoRotation
comment.TextOrientationType = TextOrientationType.NoRotation;
Console.WriteLine("Text Orientation: NoRotation");
// Save the workbook
workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");
// Change text orientation to TopToBottom
comment.TextOrientationType = TextOrientationType.TopToBottom;
Console.WriteLine("Text Orientation: TopToBottom");
// Save the workbook
workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
