---
title: "Enumeración WebExtensionStoreType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.WebExtensions.WebExtensionStoreType. Representa el tipo de almacén de la extensión web"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

Representa el tipo de almacén de la extensión web.

```csharp
public enum WebExtensionStoreType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| OMEX | `0` | Especifica que el tipo de almacén es Office.com. |
| SPCatalog | `1` | Especifica que el tipo de almacén es el catálogo corporativo de SharePoint. |
| SPApp | `2` | Especifica que el tipo de almacén es una aplicación web de SharePoint. |
| Exchange | `3` | Especifica que el tipo de almacén es un servidor Exchange. |
| FileSystem | `4` | Especifica que el tipo de almacén es un recurso compartido del sistema de archivos. |
| Registry | `5` | Especifica que el tipo de almacén es el registro del sistema. |
| ExCatalog | `6` | Especifica que el tipo de almacén es Implementación Centralizada a través de Exchange. |

### Ejemplos

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

### Ver también

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


