##HtmlLoadOptions.DeleteRedundantSpaces
HtmlLoadOptions property. Indicates whether delete redundant spaces when the text wraps lines using br tag. The default value is false
## HtmlLoadOptions.DeleteRedundantSpaces property
Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag. The default value is false.
```csharp
public bool DeleteRedundantSpaces { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlLoadOptionsPropertyDeleteRedundantSpacesDemo
{
public static void Run()
{
string html = "<p>   This    text   has   redundant   spaces   </p>";
HtmlLoadOptions opts = new HtmlLoadOptions();
opts.DeleteRedundantSpaces = true;
byte[] htmlBytes = Encoding.UTF8.GetBytes(html);
using (MemoryStream stream = new MemoryStream(htmlBytes))
{
Workbook workbook = new Workbook(stream, opts);
Worksheet worksheet = workbook.Worksheets[0];
Console.WriteLine("Cell text after removing redundant spaces: " +
worksheet.Cells["A1"].StringValue);
workbook.Save("output.xlsx");
}
}
}
}
```
### See Also
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
