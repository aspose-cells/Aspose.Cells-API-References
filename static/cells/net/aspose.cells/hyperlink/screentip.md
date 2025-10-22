##Hyperlink.ScreenTip
Hyperlink property. Returns or sets the ScreenTip text for the specified hyperlink
## Hyperlink.ScreenTip property
Returns or sets the ScreenTip text for the specified hyperlink.
```csharp
public string ScreenTip { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkPropertyScreenTipDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Click this hyperlink:");
// Create a hyperlink with ScreenTip
int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";
// Save the workbook
workbook.Save("HyperlinkWithScreenTip.xlsx");
}
}
}
```
### See Also
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
