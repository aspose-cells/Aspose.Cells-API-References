##Hyperlink.LinkType
Hyperlink property. Gets the link type
## Hyperlink.LinkType property
Gets the link type.
```csharp
public TargetModeType LinkType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkPropertyLinkTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an external hyperlink
int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
// Demonstrate LinkType property
Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
// Clean up
link.Delete();
Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
}
}
}
```
### See Also
* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
