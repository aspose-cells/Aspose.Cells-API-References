##PageSetup.PrintComments
PageSetup property. Represents the way comments are printed with the sheet
## PageSetup.PrintComments property
Represents the way comments are printed with the sheet.
```csharp
public PrintCommentsType PrintComments { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintCommentsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = sheet.Comments.Add("A1");
Comment comment = sheet.Comments[commentIndex];
comment.Note = "This is a test comment";
// Set different print comment options and demonstrate their effects
sheet.PageSetup.PrintComments = PrintCommentsType.PrintInPlace;
Console.WriteLine("PrintComments set to PrintInPlace");
sheet.PageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;
Console.WriteLine("PrintComments set to PrintSheetEnd");
sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;
Console.WriteLine("PrintComments set to PrintNoComments");
// Save the workbook to demonstrate the settings persist
workbook.Save("PrintCommentsDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [PrintCommentsType](../../printcommentstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
