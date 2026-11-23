---
title: "WebExtensionTaskPane.WebExtension"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionTaskPane. Obtient et définit la partie d'extension web associée à l'instance du taskpane"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensiontaskpane/webextension/
---
## WebExtensionTaskPane.WebExtension property

Obtient et définit la partie d'extension web associée à l'instance du volet de tâche

```csharp
public WebExtension WebExtension { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyWebExtensionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;

            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtension](../../webextension/)
* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


