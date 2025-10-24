##HtmlLoadOptions.AttachedFilesDirectory
HtmlLoadOptions property. The directory that the attached files will be saved to
## HtmlLoadOptions.AttachedFilesDirectory property
The directory that the attached files will be saved to.
```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use HtmlLoadOptions.StreamProvider property. This property will be removed 12 months later since December 2014. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
{
public static void Run()
{
// Create an instance of HtmlLoadOptions
HtmlLoadOptions options = new HtmlLoadOptions();
// Set the directory for attached files
options.AttachedFilesDirectory = "C:\\AttachedFiles";
// Load an HTML file into a Workbook using the specified options
Workbook workbook = new Workbook("input.html", options);
// Save the workbook to an Excel file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
