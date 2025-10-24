##HtmlSaveOptions.IsFullPathLink
HtmlSaveOptions property. Indicating whether using full path link in sheet00x.htmfilelist.xml and tabstrip.htm. The default value is false
## HtmlSaveOptions.IsFullPathLink property
Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.
```csharp
public bool IsFullPathLink { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyIsFullPathLinkDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test HTML Export");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Demonstrate IsFullPathLink property
saveOptions.IsFullPathLink = true; // Set to true to use full path links
// Save with different IsFullPathLink settings
workbook.Save("HtmlExport_FullPathLinks.html", saveOptions);
saveOptions.IsFullPathLink = false; // Set to false for relative paths
workbook.Save("HtmlExport_RelativeLinks.html", saveOptions);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
