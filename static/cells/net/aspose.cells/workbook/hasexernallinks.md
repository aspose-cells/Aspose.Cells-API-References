##Workbook.HasExernalLinks
Workbook method. Indicates whether this workbook contains external links to other data sources
## Workbook.HasExernalLinks method
Indicates whether this workbook contains external links to other data sources.
```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```
### Return Value
Whether this workbook contains external links to other data sources.
### Remarks
NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Count to check whether there are external links in this workbook. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodHasExernalLinksDemo
{
public static void Run()
{
// Create a workbook with external links
var workbook = new Workbook();
var worksheet = workbook.Worksheets[0];
// Add an external link
worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
// Check if workbook has external links
if (workbook.HasExernalLinks())
{
Console.WriteLine("Workbook contains external links:");
foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
{
Console.WriteLine($"External Link: {link.DataSource}");
}
}
else
{
Console.WriteLine("Workbook has no external links");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
