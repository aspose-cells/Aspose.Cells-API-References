##HtmlLoadOptions.ProgId
HtmlLoadOptions property. Gets the program id of creating the file. Only for MHT files
## HtmlLoadOptions.ProgId property
Gets the program id of creating the file. Only for MHT files.
```csharp
public string ProgId { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertyProgIdDemo
{
public static void Run()
{
// Create HTML load options with MHTML format
HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
// Get the ProgId property
Console.WriteLine("ProgId is: " + options.ProgId);
// Create another instance and get its ProgId
HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
Console.WriteLine("ProgId is: " + wordOptions.ProgId);
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
