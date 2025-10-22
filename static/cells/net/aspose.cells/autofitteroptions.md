##Class AutoFitterOptions
Aspose.Cells.AutoFitterOptions class. Represents all auto fitter options
## AutoFitterOptions class
Represents all auto fitter options.
```csharp
public class AutoFitterOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) Indicates whether auto fit row height when the cells is merged in a row. The default value is false. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | Gets and set the type of auto fitting row height of merged cells. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | Gets and sets the type of auto fitting wrapped text. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | Gets or sets default edit language. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | Gets and sets the formatted strategy. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | Indicates whether fit for rendering purpose. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | Ignores the hidden rows/columns. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | Gets and sets the max row height(in unit of Point) when autofitting rows. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | Indicates whether only fit the rows which height are not customed. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
public class AutoFitterOptionsDemo
{
public static void AutoFitterOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");
Style style = worksheet.Cells["A1"].GetStyle();
style.IsTextWrapped = true;
worksheet.Cells["A1"].SetStyle(style);
// Create a range A1:B2
Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);
// Merge the cells
range.Merge();
// Create an instance of AutoFitterOptions
AutoFitterOptions options = new AutoFitterOptions
{
DefaultEditLanguage = DefaultEditLanguage.English,
AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
OnlyAuto = true,
IgnoreHidden = true,
MaxRowHeight = 50.0,
AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
FormatStrategy = CellValueFormatStrategy.DisplayString,
ForRendering = true
};
// Apply auto fit rows with the specified options
worksheet.AutoFitRows(options);
// Save the workbook
workbook.Save("AutoFitterOptionsExample.xlsx");
workbook.Save("AutoFitterOptionsExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
