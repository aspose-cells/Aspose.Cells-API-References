##MarkdownSaveOptions.FormatStrategy
MarkdownSaveOptions property. Gets and sets the format strategy when exporting the cell value as string
## MarkdownSaveOptions.FormatStrategy property
Gets and sets the format strategy when exporting the cell value as string.
```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MarkdownSaveOptionsPropertyFormatStrategyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with different formats
worksheet.Cells["A1"].PutValue(123.456); // Numeric value
worksheet.Cells["A2"].PutValue(DateTime.Now); // Date value
worksheet.Cells["A3"].PutValue(true); // Boolean value
// Create Markdown save options with DisplayString format strategy
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
{
FormatStrategy = CellValueFormatStrategy.DisplayString
};
// Save the workbook as Markdown
workbook.Save("MarkdownWithDisplayString.md", saveOptions);
// Change to CellValueFormatStrategy.CellStyle
saveOptions.FormatStrategy = CellValueFormatStrategy.CellStyle;
workbook.Save("MarkdownWithCellStyle.md", saveOptions);
Console.WriteLine("Markdown files saved successfully with different format strategies.");
}
}
}
```
### See Also
* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
