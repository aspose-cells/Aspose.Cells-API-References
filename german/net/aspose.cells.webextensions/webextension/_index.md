---
title: "Klasse WebExtension"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WebExtensions.WebExtension-Klasse. Stellt eine Office-Add-In-Instanz dar."
type: docs
url: /de/net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Stellt eine Instanz eines Office‑Add‑Ins dar.

```csharp
public class WebExtension
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Liest eine Liste von alternativen Verweisen. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Liest alle Bindungsbeziehungen zwischen einem Office-Add-In und den Daten im Dokument. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Liest und setzt die eindeutige Kennung der Office-Add-In-Instanz im aktuellen Dokument. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Gibt an, ob der Benutzer mit dem Office-Add-In interagieren kann oder nicht. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Liest alle Eigenschaften der WebExtension. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Liest die primäre Referenz zu einem Office-Add-In. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


