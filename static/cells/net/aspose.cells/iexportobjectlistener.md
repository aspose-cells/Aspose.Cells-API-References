##Interface IExportObjectListener
Aspose.Cells.IExportObjectListener interface. Allows users to manipulate objects while exporting
## IExportObjectListener interface
Allows users to manipulate objects while exporting.
```csharp
public interface IExportObjectListener
```
## Methods
| Name | Description |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Export one object. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class CellsClassIExportObjectListenerDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
Picture picture = worksheet.Pictures[pictureIndex];
// Custom export listener implementation
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExportObjectListener = new CustomExportObjectListener();
// Save to HTML with custom listener
workbook.Save("output.html", saveOptions);
}
}
class CustomExportObjectListener : IExportObjectListener
{
private int imgIdx = 0;
public object ExportObject(ExportObjectEvent e)
{
object source = e.GetSource();
if (source is Shape)
{
Shape shape = (Shape)source;
if (shape.MsoDrawingType == MsoDrawingType.Picture)
{
string url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
imgIdx++;
return url;
}
}
return null;
}
private string SaveImage(byte[] data, int imgIdx, ImageType format)
{
// In a real implementation, you would save the image to disk here
// For demo purposes, we just return a dummy path
return $"images/image_{imgIdx}.png";
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
