##OleObject.ImageSourceFullName
OleObject property. Gets or sets the path and name of the source file for the linked image
## OleObject.ImageSourceFullName property
Gets or sets the path and name of the source file for the linked image.
```csharp
public string ImageSourceFullName { get; set; }
```
### Remarks
The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyImageSourceFullNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample PDF file to embed
byte[] pdfBytes = File.ReadAllBytes("example.pdf");
// Add an OleObject to the worksheet
int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
OleObject oleObj = worksheet.OleObjects[oleIndex];
// Set OleObject properties including ImageSourceFullName
oleObj.DisplayAsIcon = false;
oleObj.FileFormatType = FileFormatType.Pdf;
oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
oleObj.IsAutoSize = false;
oleObj.IsLink = false;
oleObj.ProgID = "Acrobat.Document.DC";
// Save the workbook
workbook.Save("OleObjectDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
