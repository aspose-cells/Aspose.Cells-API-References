##Enum HtmlOfficeMathOutputType
Aspose.Cells.HtmlOfficeMathOutputType enum. Represents how export OfficeMath to HTML
## HtmlOfficeMathOutputType enumeration
Represents how export OfficeMath to HTML.
```csharp
public enum HtmlOfficeMathOutputType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Image | `0` | Converts OfficeMath to HTML as image specified by &lt;img&gt; tag. |
| MathML | `1` | Converts OfficeMath to HTML using MathML. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class CellsClassHtmlOfficeMathOutputTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add OfficeMath to cell A1
worksheet.Cells["A1"].PutValue("=SUM(1,2)");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set OfficeMath output type to Image
saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
// Save with Image output type
workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
// Change output type to MathML
saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
// Save with MathML output type
workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
