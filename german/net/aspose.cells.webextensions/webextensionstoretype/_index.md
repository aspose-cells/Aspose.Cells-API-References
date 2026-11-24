---
title: "Aufzählung WebExtensionStoreType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WebExtensions.WebExtensionStoreType enum. Stellt den Store-Typ der Web-Erweiterung dar"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

Stellt den Speicherorttyp der Web-Erweiterung dar.

```csharp
public enum WebExtensionStoreType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| OMEX | `0` | Gibt an, dass der Store-Typ Office.com ist. |
| SPCatalog | `1` | Gibt an, dass der Store-Typ der SharePoint-Unternehmenskatalog ist. |
| SPApp | `2` | Gibt an, dass der Store-Typ eine SharePoint-Webanwendung ist. |
| Exchange | `3` | Gibt an, dass der Store-Typ ein Exchange-Server ist. |
| FileSystem | `4` | Gibt an, dass der Store-Typ eine Dateisystemfreigabe ist. |
| Registry | `5` | Gibt an, dass der Store-Typ die Systemregistrierung ist. |
| ExCatalog | `6` | Gibt an, dass der Store-Typ die zentrale Bereitstellung über Exchange ist. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


