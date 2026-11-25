---
title: "WebExtensionTaskPaneCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionTaskPaneCollection. Ottiene il task pane per l'indice specifico"
type: docs
url: /it/net/aspose.cells.webextensions/webextensiontaskpanecollection/item/
---
## WebExtensionTaskPaneCollection indexer

Ottiene il riquadro attività per l'indice specifico.

```csharp
public WebExtensionTaskPane this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

Il task pane.

### Esempi

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

            // Dimostra l'uso della proprietà Item
            WebExtensionTaskPane retrievedPane = taskPanes[paneIndex];
            Console.WriteLine($"Retrieved task pane width: {retrievedPane.Width}");

            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebExtensionTaskPane](../../webextensiontaskpane/)
* class [WebExtensionTaskPaneCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


