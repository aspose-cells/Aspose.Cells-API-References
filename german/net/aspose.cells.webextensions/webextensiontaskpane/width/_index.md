---
title: "WebExtensionTaskPane.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionTaskPane-Eigenschaft. Gibt den Standardbreitenwert für diese Taskpane-Instanz zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.webextensions/webextensiontaskpane/width/
---
## WebExtensionTaskPane.Width property

Liest und setzt den Standardbreitenwert für diese Task‑Pane‑Instanz.

```csharp
public double Width { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
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
            
            // Demonstriere die Verwendung der Width-Eigenschaft
            taskPane.Width = 350;
            
            workbook.Save("WebExtensionTaskPanePropertyWidthDemo.xlsx");
            
            Console.WriteLine("Workbook saved with task pane width set to: " + taskPane.Width);
        }
    }
}
```

### Siehe auch

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


