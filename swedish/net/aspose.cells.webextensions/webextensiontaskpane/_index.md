---
title: "Klass WebExtensionTaskPane"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WebExtensions.WebExtensionTaskPane-klass. Representerar ett beständigt taskpane‑objekt"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensiontaskpane/
---
## WebExtensionTaskPane class

Representerar ett beständigt taskpane-objekt.

```csharp
public class WebExtensionTaskPane
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | Hämtar och sätter den senast dockade platsen för detta taskpane‑objekt. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | Anger om taskpane är låst till dokumentet i UI och inte kan stängas av användaren. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | Anger om Task Pane visas som synlig som standard när dokumentet öppnas. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | Hämtar och sätter indexet, räknat från utsidan till insidan, för detta taskpane bland andra beständiga taskpanes som är dockade på samma standardplats. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | Hämtar och sätter web extension-delen som är associerad med taskpane‑instansen |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | Hämtar och sätter standardbreddvärdet för denna taskpane‑instans. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionTaskPaneDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;

            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


