##AutoFitterOptions.FormatStrategy
AutoFitterOptions property. Gets and sets the formatted strategy
## AutoFitterOptions.FormatStrategy property
Gets and sets the formatted strategy.
```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```
### Remarks
The default value is CellStyle for performance.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyFormatStrategyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data and wrap text
worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
Style style = worksheet.Cells["A1"].GetStyle();
style.IsTextWrapped = true;
worksheet.Cells["A1"].SetStyle(style);
// Create AutoFitterOptions with FormatStrategy
AutoFitterOptions options = new AutoFitterOptions
{
FormatStrategy = CellValueFormatStrategy.DisplayString,
AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
};
// Apply auto-fit with the specified options
worksheet.AutoFitRows(options);
// Save the result
workbook.Save("FormatStrategyDemo.xlsx");
}
}
}
```
### See Also
* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
