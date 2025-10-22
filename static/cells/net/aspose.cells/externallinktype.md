##Enum ExternalLinkType
Aspose.Cells.ExternalLinkType enum. Represents the type of external link
## ExternalLinkType enumeration
Represents the type of external link.
```csharp
public enum ExternalLinkType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DDELink | `0` | Represents the DDE link. |
| External | `1` | Represents external link. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ExternalLinkTypeDemo
{
public static void ExternalLinkTypeExample()
{
// Open a file with external links
Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");
// Get External Link
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
// Display the type of external link
Console.WriteLine("External Link Type: " + externalLink.Type);
// Change External Link's Data Source
externalLink.DataSource = "d:\\link.xls";
// Save the workbook
workbook.Save("ExternalLinkTypeExample.xlsx");
}
}
// Enum representing the type of external link
public enum ExternalLinkType
{
DDELink = 0, // Represents the DDE link
External = 1 // Represents external link
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
