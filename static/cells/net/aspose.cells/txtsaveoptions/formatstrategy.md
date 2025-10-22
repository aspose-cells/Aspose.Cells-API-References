##TxtSaveOptions.FormatStrategy
TxtSaveOptions property. Gets and sets the format strategy when exporting the cell value as string
## TxtSaveOptions.FormatStrategy property
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
public class TxtSaveOptionsPropertyFormatStrategyDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set values with different formats
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(999.99);
worksheet.Cells["A3"].PutValue("Phone");
worksheet.Cells["B3"].PutValue(599.99);
// Apply number format to prices
Style style = workbook.CreateStyle();
style.Number = 2; // Format as currency
worksheet.Cells["B2:B3"].SetStyle(style);
// Configure text save options with different format strategies
TxtSaveOptions options = new TxtSaveOptions
{
Separator = '\t',
FormatStrategy = CellValueFormatStrategy.DisplayStyle // Show formatted values
};
// Save with display formatting
workbook.Save("FormattedOutput.txt", options);
// Change to no formatting strategy
options.FormatStrategy = CellValueFormatStrategy.None;
workbook.Save("RawOutput.txt", options);
Console.WriteLine("Files saved with different format strategies.");
}
}
}
```
### See Also
* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
