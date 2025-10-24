##Name.Comment
Name property. Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions
## Name.Comment property
Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions.
```csharp
public string Comment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NamePropertyCommentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a named range with comment
int index = workbook.Worksheets.Names.Add("TestRange");
Name namedRange = workbook.Worksheets.Names[index];
namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
namedRange.Comment = "This is a test named range";
// Save the workbook
workbook.Save("NamedRangeWithComment.xlsx");
// Load the saved workbook to verify the comment
Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
// Output the comment to demonstrate functionality
Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
