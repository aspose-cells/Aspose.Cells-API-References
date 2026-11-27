---
title: "Klass WebExtension"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WebExtensions.WebExtension class. Representerar en Office-tilläggsinstans"
type: docs
url: /sv/net/aspose.cells.webextensions/webextension/
---
## WebExtension class

Representerar en Office-tilläggsinstans.

```csharp
public class WebExtension
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | Hämtar en lista över alter-referenser. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | Hämtar alla bindningsförhållanden mellan ett Office-tillägg och data i dokumentet. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | Hämtar och anger den unika identifieraren för Office-tilläggets instans i det aktuella dokumentet. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | Anger om användaren kan interagera med Office-tillägget eller inte. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | Hämtar alla egenskaper för web extension. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | Hämta den primära referensen till ett Office-tillägg. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


