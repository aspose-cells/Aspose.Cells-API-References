##ExternalLink.OriginalDataSource
ExternalLink property. Represents stored data source of the external link
## ExternalLink.OriginalDataSource property
Represents stored data source of the external link.
```csharp
public string OriginalDataSource { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkPropertyOriginalDataSourceDemo
{
public static void Run()
{
// Create a workbook with external links
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add external link
worksheet.Cells["A1"].Formula = "='https://arcusventures.sharepoint.com/Fund II/[example.xlsx]Sheet1'!A1";
// Modify external link paths
for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
{
string originalLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
string modifiedLink = originalLink.Replace(
@"https://arcusventures.sharepoint.com/Fund II/",
@"/sites/shared/shared documents/Fund II/");
workbook.Worksheets.ExternalLinks[i].OriginalDataSource = modifiedLink;
}
// Verify the changes
foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
{
Console.WriteLine("Modified Link: " + link.OriginalDataSource);
}
}
}
}
```
### See Also
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
