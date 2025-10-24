##ExternalLink.IsReferred
ExternalLink property. Indicates whether this external link is referenced by others
## ExternalLink.IsReferred property
Indicates whether this external link is referenced by others.
```csharp
public bool IsReferred { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkPropertyIsReferredDemo
{
public static void Run()
{
// Create a workbook with external link
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add external link reference
worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
// Check if the external link is referred
if (workbook.Worksheets.ExternalLinks.Count > 0)
{
bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
Console.WriteLine("Is external link referred: " + isReferred);
}
}
}
}
```
### See Also
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
