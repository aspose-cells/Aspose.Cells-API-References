##Enum ImageType
Aspose.Cells.Drawing.ImageType enum. Specifies the type format of an image
## ImageType enumeration
Specifies the type (format) of an image.
```csharp
public enum ImageType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Unknown | `0` | An unknown image type. |
| Emf | `2` | Windows Enhanced Metafile. |
| Wmf | `3` | Windows Metafile. |
| Pict | `4` | Macintosh PICT. |
| Jpeg | `5` | JPEG JFIF. |
| Png | `6` | Portable Network Graphics. |
| Bmp | `7` | Windows Bitmap |
| Gif | `66` | Gif |
| Tiff | `67` | Tiff |
| Svg | `68` | Svg |
| Svm | `69` | Svm |
| Gltf | `70` | glTF |
| OfficeCompatibleEmf | `71` | Windows Enhanced Metafile which is more compatible with Office. |
| WebP | `72` | Weppy image format |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class ImageTypeDemo
{
public static void ImageTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Save the chart as an image in different formats
chart.ToImage("ChartImageEmf.emf", ImageType.Emf);
chart.ToImage("ChartImageWmf.wmf", ImageType.Wmf);
chart.ToImage("ChartImagePng.png", ImageType.Png);
chart.ToImage("ChartImageJpeg.jpeg", ImageType.Jpeg);
chart.ToImage("ChartImageBmp.bmp", ImageType.Bmp);
chart.ToImage("ChartImageGif.gif", ImageType.Gif);
chart.ToImage("ChartImageTiff.tiff", ImageType.Tiff);
chart.ToImage("ChartImageSvg.svg", ImageType.Svg);
// Output the results
Console.WriteLine("Chart images saved in various formats.");
// Save the workbook
workbook.Save("ImageTypeExample.xlsx");
workbook.Save("ImageTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
