##StyleFlag.QuotePrefix
StyleFlag property. Hide formula setting will be applied
## StyleFlag.QuotePrefix property
Hide formula setting will be applied.
```csharp
public bool QuotePrefix { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StyleFlagPropertyQuotePrefixDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set a value that looks like a number but should be treated as text
Cell cell = worksheet.Cells["A1"];
cell.PutValue("123456");
// Create a style and set QuotePrefix to true
Style style = workbook.CreateStyle();
style.QuotePrefix = true;
// Create a style flag and enable QuotePrefix flag
StyleFlag flag = new StyleFlag();
flag.QuotePrefix = true;
// Apply the style to the cell using SetStyle instead of ApplyStyle
cell.SetStyle(style, flag);
// Display the current QuotePrefix value
Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
// Save the workbook to see the effect (the value will be treated as text in Excel)
workbook.Save("PropertyQuotePrefixDemo.xlsx");
// Now let's change the QuotePrefix to false and see the difference
style.QuotePrefix = false;
cell.SetStyle(style, flag);
Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
// Save again with different name to compare
workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
