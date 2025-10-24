##Class ExportObjectEvent
Aspose.Cells.ExportObjectEvent class. The event triggered when exporting an object such as Picture
## ExportObjectEvent class
The event triggered when exporting an object, such as Picture.
```csharp
public class ExportObjectEvent
```
## Methods
| Name | Description |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | Gets the object to be exported. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class ExportObjectEventDemo
{
public static void ExportObjectEventExample()
{
// Custom implementation of IExportObjectListener
// Save HTML file with custom listener
Workbook workbook = new Workbook(); // Build your workbook here
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
ExportObjectListener = new CustomExportObjectListener()
};
using (Stream stream = new FileStream("ExportObjectEventExample.html", FileMode.Create))
{
workbook.Save(stream, saveOptions); // Save the workbook to stream
}
}
}
class CustomExportObjectListener : IExportObjectListener
{
private int imgIdx = 0;
public object ExportObject(ExportObjectEvent e)
{
object source = e.GetSource();
if (source is Shape shape)
{
string url = null;
switch (shape.MsoDrawingType)
{
case MsoDrawingType.Picture:
url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
break;
}
if (url != null)
{
imgIdx++;
}
return url;
}
return null;
}
private string SaveImage(byte[] data, int imgIdx, ImageType format)
{
// Here save the image to any location, then return the URL (relative or absolute) that the generated HTML can get the image
return $"temp{imgIdx}/temp{imgIdx}.png";
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
