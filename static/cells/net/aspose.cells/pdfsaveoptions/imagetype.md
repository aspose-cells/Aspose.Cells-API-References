##PdfSaveOptions.ImageType
PdfSaveOptions property. Represents the image type when converting the chart and shape
## PdfSaveOptions.ImageType property
Represents the image type when converting the chart and shape .
```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
using System.Drawing.Imaging;
public class PdfSaveOptionsPropertyImageTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample image to the worksheet
int imageIndex = worksheet.Pictures.Add(0, 0, "sample.jpg");
Picture picture = worksheet.Pictures[imageIndex];
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Display the current ImageType value (default is Unknown)
Console.WriteLine("Current ImageType value: " + pdfSaveOptions.ImageType);
// Set the image type to JPEG for PDF conversion
pdfSaveOptions.ImageType = ImageFormat.Jpeg;
// Demonstrate the effect by saving to PDF
workbook.Save("PropertyImageTypeDemo.pdf", pdfSaveOptions);
// Change the image type to PNG and save again
pdfSaveOptions.ImageType = ImageFormat.Png;
workbook.Save("PropertyImageTypeDemo_Png.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
