##ImageOrPrintOptions.VerticalResolution
ImageOrPrintOptions property. Gets or sets the vertical resolution for generated images in dots per inch
## ImageOrPrintOptions.VerticalResolution property
Gets or sets the vertical resolution for generated images, in dots per inch.
```csharp
public int VerticalResolution { get; set; }
```
### Remarks
The default value is 96.
Setting [`HorizontalResolution`](../horizontalresolution/) and `VerticalResolution` effects the width and height of the output image in pixels.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyVerticalResolutionDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and create a chart
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B3"].PutValue(200);
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Create image options with specific vertical resolution
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = ImageType.Png;
options.VerticalResolution = 300; // Setting vertical resolution to 300 DPI
options.HorizontalResolution = 300; // For consistency, setting horizontal resolution too
// Save chart as image with specified resolution
chart.ToImage("output_chart.png", options);
Console.WriteLine("Chart saved as image with vertical resolution of 300 DPI.");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
