##Range.AddHyperlink
Range method. Adds a hyperlink to a specified cell or a range of cells
## Range.AddHyperlink method
Adds a hyperlink to a specified cell or a range of cells.
```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```
| Parameter | Type | Description |
| --- | --- | --- |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |
### Return Value
[`Hyperlink`](../../hyperlink/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodAddHyperlinkWithStringStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
// Add hyperlink with address, text to display and screen tip
range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
// Save the workbook
workbook.Save("HyperlinkDemo.xlsx");
}
}
}
```
### See Also
* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
