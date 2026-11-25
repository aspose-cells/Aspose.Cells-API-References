---
title: "Enum WebExtensionStoreType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.WebExtensions.WebExtensionStoreType enum. Rappresenta il tipo di archivio dell'estensione web"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

Rappresenta il tipo di archivio dell'estensione web.

```csharp
public enum WebExtensionStoreType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| OMEX | `0` | Specifica che il tipo di archivio è Office.com. |
| SPCatalog | `1` | Specifica che il tipo di archivio è il catalogo aziendale SharePoint. |
| SPApp | `2` | Specifica che il tipo di archivio è un'applicazione web SharePoint. |
| Exchange | `3` | Specifica che il tipo di archivio è un server Exchange. |
| FileSystem | `4` | Specifica che il tipo di archivio è una condivisione del file system. |
| Registry | `5` | Specifica che il tipo di archivio è il registro di sistema. |
| ExCatalog | `6` | Specifica che il tipo di archivio è la distribuzione centralizzata tramite Exchange. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


