##HtmlSaveOptions.CellCssPrefix
HtmlSaveOptions property. Gets and sets the prefix of the css namethe default value is
## HtmlSaveOptions.CellCssPrefix property
Gets and sets the prefix of the css name,the default value is "".
```csharp
public string CellCssPrefix { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyCellCssPrefixDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
// Set HTML save options with CellCssPrefix
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.CellCssPrefix = "custom-cell-";
// Save the workbook with HTML options
workbook.Save("output.html", saveOptions);
Console.WriteLine("HTML file saved with custom cell CSS prefix.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
