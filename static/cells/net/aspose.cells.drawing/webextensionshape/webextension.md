##WebExtensionShape.WebExtension
WebExtensionShape property. Gets and set the web extension
## WebExtensionShape.WebExtension property
Gets and set the web extension.
```csharp
public WebExtension WebExtension { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionShapePropertyWebExtensionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int index = webExtensions.Add();
WebExtension webExt = webExtensions[index];
webExt.Reference.Id = "wa104104476";
webExt.Reference.Version = "1.3.0.0";
webExt.Reference.StoreName = "en-US";
webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
webExt.Properties.Add("sku", "peoplebar-giant");
webExt.Properties.Add("theme", "giant-redwhiteblack");
webExt.Properties.Add("shape", "muscle-people");
webExt.Properties.Add("layout-element-title", "NUMBERS ABOUT THE APP");
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 500, 500, 100, 100);
WebExtensionShape wShape = (WebExtensionShape)shapes[0];
wShape.WebExtension = webExt;
workbook.Save("WebExtensionDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtension](../../../aspose.cells.webextensions/webextension/)
* class [WebExtensionShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
