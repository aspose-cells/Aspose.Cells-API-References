---
title: "Enum WebExtensionStoreType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WebExtensions.WebExtensionStoreType-enum. Representerar lagringstypen för webbtillägg"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

Representerar lagringstypen för webbutökning.

```csharp
public enum WebExtensionStoreType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| OMEX | `0` | Anger att lagringstypen är Office.com. |
| SPCatalog | `1` | Anger att lagringstypen är SharePoint företagskatalog. |
| SPApp | `2` | Anger att lagringstypen är en SharePoint webbapplikation. |
| Exchange | `3` | Anger att lagringstypen är en Exchange-server. |
| FileSystem | `4` | Anger att lagringstypen är en fildelningsresurs. |
| Registry | `5` | Anger att lagringstypen är systemregistret. |
| ExCatalog | `6` | Anger att lagringstypen är Centraliserad distribution via Exchange. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


