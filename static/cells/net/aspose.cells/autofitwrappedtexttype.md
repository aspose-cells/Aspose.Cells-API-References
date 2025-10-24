##Enum AutoFitWrappedTextType
Aspose.Cells.AutoFitWrappedTextType enum. Represents the type of auto fitting wrapped text
## AutoFitWrappedTextType enumeration
Represents the type of auto fitting wrapped text.
```csharp
public enum AutoFitWrappedTextType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Works as MS Excel. |
| Paragraph | `1` | Auto fit width with the longest paragraph. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
public class AutoFitWrappedTextTypeDemo
{
public static void AutoFitWrappedTextTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");
Style style = worksheet.Cells["A1"].GetStyle();
style.IsTextWrapped = true;
worksheet.Cells["A1"].SetStyle(style);
Style style2 = worksheet.Cells["A5"].GetStyle();
style2.IsTextWrapped = true;
worksheet.Cells["A5"].SetStyle(style);
// Create a range A1:F3
Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
// Merge the cells
range.Merge();
// Create a range A4:F6
Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
// Merge the cells
range2.Merge();
// Create AutoFitterOptions and set AutoFitWrappedTextType
AutoFitterOptions options = new AutoFitterOptions();
options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;
// Auto-fit rows with the specified options
worksheet.AutoFitRows(options);
// Save the workbook
workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
workbook.Save("AutoFitWrappedTextTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
