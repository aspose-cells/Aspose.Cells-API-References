##DataBar.ToImage
DataBar method. Render data bar in cell to image byte array
## DataBar.ToImage method
Render data bar in cell to image byte array.
```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Indicate the data bar in which cell to be rendered |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class DataBarMethodToImageWithCellImageOrPrintOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and conditional formatting
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Add data bar conditional formatting
int idx = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 3;
area.EndColumn = 0;
fcc.AddArea(area);
idx = fcc.AddCondition(FormatConditionType.DataBar);
FormatCondition cond = fcc[idx];
cond.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
cond.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
// Get the cell with conditional formatting
Cell cell = worksheet.Cells["A1"];
ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
if (result != null && result.ConditionalFormattingDataBar != null)
{
DataBar bar = result.ConditionalFormattingDataBar;
ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
// Convert data bar to image
byte[] img = bar.ToImage(cell, imgOpts);
// Save the image
string outputPath = "DataBarImage.png";
File.WriteAllBytes(outputPath, img);
// For image verification, you would need to add System.Drawing.Common package
// and use System.Drawing.Image if needed
Console.WriteLine($"Data bar image saved to {outputPath}");
}
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
