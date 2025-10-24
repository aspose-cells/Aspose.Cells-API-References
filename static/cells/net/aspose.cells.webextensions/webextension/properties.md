##WebExtension.Properties
WebExtension property. Gets all properties of web extension
## WebExtension.Properties property
Gets all properties of web extension.
```csharp
public WebExtensionPropertyCollection Properties { get; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionPropertyPropertiesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
int extIndex = workbook.Worksheets.WebExtensions.Add();
WebExtension webExt = workbook.Worksheets.WebExtensions[extIndex];
webExt.Reference.Id = "wa104104476";
webExt.Reference.Version = "1.3.0.0";
webExt.Reference.StoreName = "en-US";
webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
webExt.Properties.Add("theme", "\"giant-redwhiteblack\"");
webExt.Properties.Add("sku", "\"peoplebar-giant\"");
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
WebExtensionShape webShape = (WebExtensionShape)shapes[0];
webShape.WebExtension = webExt;
workbook.Save("WebExtensionPropertyPropertiesDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionPropertyCollection](../../webextensionpropertycollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
