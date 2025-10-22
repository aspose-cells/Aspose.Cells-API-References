##HyperlinkCollection.Item
HyperlinkCollection property. Gets the Hyperlink element at the specified index
## HyperlinkCollection indexer
Gets the [`Hyperlink`](../../hyperlink/) element at the specified index.
```csharp
public Hyperlink this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a hyperlink to cell A1
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
// Access the first hyperlink using Item property and set display text
worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
// Set hyperlink style (blue underlined text)
Style style = worksheet.Cells["A1"].GetStyle();
style.Font.Color = System.Drawing.Color.Blue;
style.Font.Underline = FontUnderlineType.Single;
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("HyperlinkExample.xlsx");
}
}
}
```
### See Also
* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
