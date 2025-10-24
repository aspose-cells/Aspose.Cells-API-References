##Enum WebExtensionStoreType
Aspose.Cells.WebExtensions.WebExtensionStoreType enum. Represents the store type of web extension
## WebExtensionStoreType enumeration
Represents the store type of web extension.
```csharp
public enum WebExtensionStoreType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| OMEX | `0` | Specifies that the store type is Office.com. |
| SPCatalog | `1` | Specifies that the store type is SharePoint corporate catalog. |
| SPApp | `2` | Specifies that the store type is a SharePoint web application. |
| Exchange | `3` | Specifies that the store type is an Exchange server. |
| FileSystem | `4` | Specifies that the store type is a file system share. |
| Registry | `5` | Specifies that the store type is the system registry. |
| ExCatalog | `6` | Specifies that the store type is Centralized Deployment via Exchange. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WebExtensionsClassWebExtensionStoreTypeDemo
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
webExt.Properties.Add("sku", "\"peoplebar-giant\"");
webExt.Properties.Add("theme", "\"giant-redwhiteblack\"");
webExt.Properties.Add("shape", "\"muscle-people\"");
webExt.Properties.Add("layout-element-title", "\"NUMBERS ABOUT THE APP\"");
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
WebExtensionShape wShape = (WebExtensionShape)shapes[0];
wShape.WebExtension = webExt;
workbook.Save("WebExtensionStoreTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)
