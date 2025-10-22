##HtmlSaveOptions.EncodeEntityAsCode
HtmlSaveOptions property. Indicates whether the html character entities are replaced with decimal code. e.g. nbsp is replaced with 160. The default value is false
## HtmlSaveOptions.EncodeEntityAsCode property
Indicates whether the html character entities are replaced with decimal code. (e.g. "&amp;nbsp;" is replaced with "&amp;#160;"). The default value is false.
```csharp
public bool EncodeEntityAsCode { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with special characters
worksheet.Cells["A1"].PutValue("Sample & Text");
worksheet.Cells["A2"].PutValue("Another <Test> String");
worksheet.Cells["A3"].PutValue("Price: $100");
// Create HTML save options
HtmlSaveOptions options = new HtmlSaveOptions();
// Display current value of EncodeEntityAsCode
Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);
// Set EncodeEntityAsCode to true
options.EncodeEntityAsCode = true;
// Save with entities encoded as code
workbook.Save("HtmlWithEncodedEntities.html", options);
// Set EncodeEntityAsCode to false
options.EncodeEntityAsCode = false;
// Save with entities as-is
workbook.Save("HtmlWithRawEntities.html", options);
// Compare the output files
Console.WriteLine("Files created:");
Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
