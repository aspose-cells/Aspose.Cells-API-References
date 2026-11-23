---
title: "WebExtensionTaskPane.DockState"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionTaskPane. Obtient et définit l'emplacement lastdocked de cet objet taskpane"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensiontaskpane/dockstate/
---
## WebExtensionTaskPane.DockState property

Obtient et définit le dernier emplacement ancré de cet objet de volet de tâche.

```csharp
public string DockState { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyDockStateDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Temp\\Addins\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right"; // Demonstrating DockState property
            taskPane.IsVisible = true;
            taskPane.Width = 300;

            workbook.Save("WebExtensionTaskPaneDockStateDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


