---
title: "Clase WebExtension"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.WebExtensions.WebExtension class. Representa una instancia de complemento de Office"
type: docs
url: /es/net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Representa una instancia de Office Add-in.

```csharp
public class WebExtension
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Obtiene una lista de alter references. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Obtiene todas las relaciones de enlaces entre un Office Add-in y los datos del documento. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Obtiene y establece la identificación única de la instancia del Office Add-in en el documento actual. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Indica si el usuario puede interactuar con el Office Add-in o no. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Obtiene todas las propiedades de la extensión web. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Obtiene la referencia principal a un Office Add-in. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "YouTube";
            
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 410, 730);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


