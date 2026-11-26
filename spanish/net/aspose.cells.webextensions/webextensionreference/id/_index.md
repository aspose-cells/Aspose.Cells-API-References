---
title: "WebExtensionReference.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionReference. Obtiene y establece el identificador asociado con el Office Addin dentro de un proveedor de catálogo. El identificador DEBE ser único dentro de un proveedor de catálogo"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

Obtiene y establece el identificador asociado con el complemento de Office dentro de un proveedor de catálogo. El identificador DEBE ser único dentro de un proveedor de catálogo.

```csharp
public string Id { get; set; }
```

### Ejemplos

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
            
            // Configurando la propiedad Id y otras propiedades de referencia
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Añadiendo propiedades de la extensión web
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            // Añadiendo forma y vinculando la extensión web
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            // Guardar y verificar
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


