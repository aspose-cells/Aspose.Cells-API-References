##Worksheet.ClearComments
Worksheet method. Clears all comments in designer spreadsheet
## Worksheet.ClearComments method
Clears all comments in designer spreadsheet.
```csharp
public void ClearComments()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodClearCommentsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample comments to cells using cell references
int comment1 = worksheet.Comments.Add("A1");
worksheet.Comments[comment1].Note = "This is comment 1";
int comment2 = worksheet.Comments.Add("B3");
worksheet.Comments[comment2].Note = "This is comment 2";
int comment3 = worksheet.Comments.Add("C5");
worksheet.Comments[comment3].Note = "This is comment 3";
// Display comment count before clearing
Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");
// Clear all comments from the worksheet
worksheet.ClearComments();
// Display comment count after clearing
Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");
// Save the workbook
workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
