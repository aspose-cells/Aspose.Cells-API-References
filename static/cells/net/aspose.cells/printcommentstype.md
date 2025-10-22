##Enum PrintCommentsType
Aspose.Cells.PrintCommentsType enum. Represents the way comments are printed with the sheet
## PrintCommentsType enumeration
Represents the way comments are printed with the sheet.
```csharp
public enum PrintCommentsType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| PrintInPlace | `0` | Represents to print comments as displayed on sheet. |
| PrintNoComments | `1` | Represents not to print comments. |
| PrintSheetEnd | `2` | Represents to print comments at end of sheet. |
| PrintWithThreadedComments | `3` | Represents to print comments as displayed on sheet include threaded comments. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class PrintCommentsTypeDemo
{
public static void PrintCommentsTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some comments to the worksheet
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a comment.";
commentIndex = worksheet.Comments.Add("B2");
comment = worksheet.Comments[commentIndex];
comment.Note = "This is another comment.";
// Set the print comments type in the page setup
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;
// Save the workbook to a file
workbook.Save("PrintCommentsTypeExample.xlsx");
Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
