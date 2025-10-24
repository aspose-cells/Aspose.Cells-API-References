##WebExtensionReference.Id
WebExtensionReference property. Gets and sets the identifier associated with the Office Addin within a catalog provider. The identifier MUST be unique within a catalog provider
## WebExtensionReference.Id property
Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider.
```csharp
public string Id { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WebExtensionReferencePropertyIdDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
int index = webExtensions.Add();
WebExtension webExt = webExtensions[index];
// Setting the Id property and other reference properties
webExt.Reference.Id = "wa104104476";
webExt.Reference.Version = "1.3.0.0";
webExt.Reference.StoreName = "en-US";
webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
// Adding web extension properties
webExt.Properties.Add("sku", "peoplebar-giant");
webExt.Properties.Add("theme", "giant-redwhiteblack");
// Adding shape and binding web extension
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
WebExtensionShape wShape = (WebExtensionShape)shapes[0];
wShape.WebExtension = webExt;
// Save and verify
workbook.Save("web_extension_demo.xlsx");
}
}
}
```
### See Also
* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
