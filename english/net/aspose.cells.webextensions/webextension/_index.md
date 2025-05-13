---
title: Class WebExtension
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WebExtensions.WebExtension class. Represents an Office Addin instance
type: docs
url: /net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Represents an Office Add-in instance.

```csharp
public class WebExtension
```

## Properties

| Name | Description |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Gets a list of alter references. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Gets all bindings relationship between an Office Add-in and the data in the document. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Indicates whether the user can interact with the Office Add-in or not. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Gets all properties of web extension. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Get the primary reference to an Office Add-in. |

### Examples

```csharp
// Called: WebExtension webExt = webExtensions[index];
public void WebExtensions_Type_WebExtension()
{
    Workbook workbook = new Workbook();
    WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
    int index = webExtensions.AddWebVideoPlayer("https://www.youtube.com/watch?v=z0hFbzPPfm8", true, 0, 0);
    WebExtension webExt = webExtensions[index];
    ShapeCollection shapes = workbook.Worksheets[0].Shapes;
    shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 410, 730);
    WebExtensionShape wShape = (WebExtensionShape)shapes[0];
    wShape.WebExtension = webExt;
    workbook.Save(Constants.destPath + "InsertYoutubeToExcel.xlsx");
}
```

### See Also

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


