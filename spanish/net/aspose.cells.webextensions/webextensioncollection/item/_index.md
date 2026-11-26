---
title: "WebExtensionCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionCollection. Obtiene la extensión web por el índice específico"
type: docs
url: /es/net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

Obtiene la extensión web por el índice específico.

```csharp
public WebExtension this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

La extensión web.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener la colección de extensiones web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // Agregar una extensión de reproductor de video web
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "youtube.com";
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            // Agregar una forma para contener la extensión web
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            // Asignar la extensión web a la forma
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // Guarda el libro de trabajo
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


