##WebExtensionCollection.Item
WebExtensionCollection property. Gets web extension by the specific index
## WebExtensionCollection indexer
Gets web extension by the specific index.
```csharp
public WebExtension this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
The web extension.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;
namespace AsposeCellsExamples
{
public class WebExtensionCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the web extensions collection
WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
// Add a web video player extension
int index = webExtensions.Add();
WebExtension webExt = webExtensions[index];
webExt.Reference.Id = "youtube";
webExt.Reference.StoreName = "youtube.com";
webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
// Add a shape to hold the web extension
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
// Assign the web extension to the shape
WebExtensionShape wShape = (WebExtensionShape)shapes[0];
wShape.WebExtension = webExt;
// Save the workbook
workbook.Save("WebExtensionDemo.xlsx");
}
}
}
```
### See Also
* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)
