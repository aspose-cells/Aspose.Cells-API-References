---
title: "WebExtensionReference.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionReference. Ottiene e imposta l'identificatore associato all'Office Addin all'interno di un provider di catalogo. L'identificatore DEVE essere unico all'interno di un provider di catalogo"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

Ottiene e imposta l'identificatore associato all'Office Add-in all'interno di un provider di catalogo. L'identificatore DEVE essere unico all'interno di un provider di catalogo.

```csharp
public string Id { get; set; }
```

### Esempi

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
            
            // Impostazione della proprietà Id e altre proprietà di riferimento
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Aggiunta di proprietà dell'estensione web
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            // Aggiunta di forma e collegamento dell'estensione web
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            // Salva e verifica
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


