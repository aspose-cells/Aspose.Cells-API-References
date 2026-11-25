---
title: "WebExtensionReference.StoreType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionReference. Ottiene e imposta il tipo di marketplace che identifica l'attributo store"
type: docs
url: /it/net/aspose.cells.webextensions/webextensionreference/storetype/
---
## WebExtensionReference.StoreType property

Ottiene e imposta il tipo di marketplace che l'attributo store identifica.

```csharp
public WebExtensionStoreType StoreType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionReferencePropertyStoreTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\server\path\to\addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;

            workbook.Save("WebExtensionStoreTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [WebExtensionStoreType](../../webextensionstoretype/)
* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


