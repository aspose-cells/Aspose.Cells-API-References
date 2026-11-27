---
title: "WebExtensionTaskPaneCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionTaskPaneCollection egenskap. Hämtar uppgiftspanel med det specifika indexet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensiontaskpanecollection/item/
---
## WebExtensionTaskPaneCollection indexer

Hämtar task pane efter det specifika indexet.

```csharp
public WebExtensionTaskPane this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Uppgiftspanelen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPaneCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpane", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;

            // Demonstrera användning av Item-egenskapen
            WebExtensionTaskPane retrievedPane = taskPanes[paneIndex];
            Console.WriteLine($"Retrieved task pane width: {retrievedPane.Width}");

            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionTaskPane](../../webextensiontaskpane/)
* class [WebExtensionTaskPaneCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


