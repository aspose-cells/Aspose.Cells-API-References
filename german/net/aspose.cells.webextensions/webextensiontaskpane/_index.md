---
title: "Klasse WebExtensionTaskPane"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WebExtensions.WebExtensionTaskPane Klasse. Stellt ein persistentes Task‑Pane‑Objekt dar"
type: docs
url: /de/net/aspose.cells.webextensions/webextensiontaskpane/
---
## WebExtensionTaskPane class

Stellt ein persistentes Taskpane-Objekt dar.

```csharp
public class WebExtensionTaskPane
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | Liest und setzt den zuletzt angedockten Ort dieses Task‑Pane‑Objekts. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | Gibt an, ob das Task‑Pane im UI an das Dokument gesperrt ist und vom Benutzer nicht geschlossen werden kann. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | Gibt an, ob das Task‑Pane standardmäßig beim Öffnen des Dokuments sichtbar ist. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | Liest und setzt den Index (von außen nach innen gezählt) dieses Task‑Pane im Vergleich zu anderen persistenten Task‑Panes, die am selben Standardort angedockt sind. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | Liest und setzt den Web‑Extension‑Teil, der mit der Task‑Pane‑Instanz verknüpft ist |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | Liest und setzt den Standardbreitenwert für diese Task‑Pane‑Instanz. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


