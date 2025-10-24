##Workbook.AbsolutePath
Workbook property. Gets and sets the absolute path of the file
## Workbook.AbsolutePath property
Gets and sets the absolute path of the file.
```csharp
public string AbsolutePath { get; set; }
```
### Remarks
Only used for external links.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyAbsolutePathDemo
{
public static void Run()
{
// Create a new workbook
Workbook sourceBook = new Workbook();
// Add some worksheets
sourceBook.Worksheets.Add("Sheet1");
sourceBook.Worksheets.Add("Sheet2");
// Save the workbook to get a physical path
string sourcePath = Path.GetFullPath("output");
if (!Directory.Exists(sourcePath))
{
Directory.CreateDirectory(sourcePath);
}
string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
sourceBook.Save(sourceFilePath);
// Reopen the workbook to demonstrate AbsolutePath
Workbook reopenedBook = new Workbook(sourceFilePath);
// Use AbsolutePath property to construct full path
string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
Console.WriteLine("Full path to workbook: " + pathToBook);
// Add hyperlinks using the path
SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");
// Save the modified workbook
string destPath = Path.Combine(sourcePath, "modified_example.xlsx");
reopenedBook.Save(destPath);
}
private static void SetHyperlink(Worksheet sheet, int linkIndex, string path, string sheetName, string cellRef)
{
HyperlinkCollection hyperlinks = sheet.Hyperlinks;
hyperlinks.Add(cellRef, 1, 1, path + "#" + sheetName + "!A1");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
