---
title: "WebExtensionReference.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionReference‑egenskap. Hämtar och anger identifieraren som är associerad med Office‑tillägget inom en katalogleverantör. Identifieraren MÅSTE vara unik inom en katalogleverantör"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

Hämtar och anger identifieraren som är associerad med Office-tillägget inom en katalogleverantör. Identifieraren MÅSTE vara unik inom en katalogleverantör.

```csharp
public string Id { get; set; }
```

### Exempel

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
            
            // Ställa in Id-egenskapen och andra referensegenskaper
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Lägger till egenskaper för web extension
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            // Lägger till form och binder web extension
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            // Spara och verifiera
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


