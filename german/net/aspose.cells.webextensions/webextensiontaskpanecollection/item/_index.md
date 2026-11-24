---
title: "WebExtensionTaskPaneCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionTaskPaneCollection-Eigenschaft. Gibt das Aufgabenfeld anhand des angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.webextensions/webextensiontaskpanecollection/item/
---
## WebExtensionTaskPaneCollection indexer

Liefert das Task-Pane anhand des angegebenen Index.

```csharp
public WebExtensionTaskPane this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Das Aufgabenfeld.

### Beispiele

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

            // Demonstriere die Verwendung der Item-Eigenschaft
            WebExtensionTaskPane retrievedPane = taskPanes[paneIndex];
            Console.WriteLine($"Retrieved task pane width: {retrievedPane.Width}");

            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionTaskPane](../../webextensiontaskpane/)
* class [WebExtensionTaskPaneCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


