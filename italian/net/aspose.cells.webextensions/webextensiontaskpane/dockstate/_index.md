---
title: "WebExtensionTaskPane.DockState"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebExtensionTaskPane. Ottiene e imposta la posizione lastdocked di questo oggetto taskpane"
type: docs
url: /it/net/aspose.cells.webextensions/webextensiontaskpane/dockstate/
---
## WebExtensionTaskPane.DockState property

Ottiene e imposta l'ultima posizione di aggancio di questo oggetto taskpane.

```csharp
public string DockState { get; set; }
```

### Esempi

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

### Vedi anche

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


