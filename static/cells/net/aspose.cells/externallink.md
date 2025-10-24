##Class ExternalLink
Aspose.Cells.ExternalLink class. Represents an external link in a workbook
## ExternalLink class
Represents an external link in a workbook.
```csharp
public class ExternalLink
```
## Properties
| Name | Description |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Represents data source of the external link. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Indicates whether this external link is referenced by others. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Indicates whether this external link is visible in MS Excel. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Represents stored data source of the external link. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | Get the path type of this external link |
| [Type](../../aspose.cells/externallink/type/) { get; } | Gets the type of external link. |
## Methods
| Name | Description |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Adds an external name. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ExternalLinkDemo
{
public static void ExternalLinkExample()
{
// Open a file with external links
Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");
// Get External Link
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
// Display properties of the external link
Console.WriteLine("External Link Type: " + externalLink.Type);
Console.WriteLine("Path Type: " + externalLink.PathType);
Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
Console.WriteLine("Data Source: " + externalLink.DataSource);
Console.WriteLine("Is Referred: " + externalLink.IsReferred);
Console.WriteLine("Is Visible: " + externalLink.IsVisible);
// Change External Link's Data Source
externalLink.DataSource = "d:\\linktest.xls";
// Add an external name to the external link
externalLink.AddExternalName("ExternalName", "Sheet1!A1");
// Save the workbook
workbook.Save("UpdatedExternalLinkExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
