---
title: "WebExtensionReference.Version"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionReference. Obtiene y establece la versión"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionreference/version/
---
## WebExtensionReference.Version property

Obtiene y establece la versión.

```csharp
public string Version { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionReferencePropertyVersionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0"; // Demonstrating Version property usage
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            workbook.Save("WebExtensionVersionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


