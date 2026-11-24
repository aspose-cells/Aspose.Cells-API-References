---
title: "WebExtensionReference.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionReference‑Eigenschaft. Gibt den Bezeichner zurück und legt ihn fest, der mit dem Office‑Add‑In innerhalb eines Katalog‑Anbieters verknüpft ist. Der Bezeichner MUSS innerhalb eines Katalog‑Anbieters eindeutig sein."
type: docs
url: /de/net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

Liest und schreibt den Bezeichner, der dem Office-Add-in innerhalb eines Kataloganbieters zugeordnet ist. Der Bezeichner MUSS innerhalb eines Kataloganbieters eindeutig sein.

```csharp
public string Id { get; set; }
```

### Beispiele

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
            
            // Festlegen der Id-Eigenschaft und anderer Referenzeigenschaften
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Hinzufügen von WebExtension-Eigenschaften
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            // Hinzufügen von Shape und Bindungs-WebExtension
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            // Speichern und überprüfen
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


