---
title: "WebExtensionTaskPane.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionTaskPane-Eigenschaft. Gibt den Index zurück und legt ihn fest, der von außen nach innen dieses Taskpanes unter anderen persistierten Taskpanes, die am selben Standardort angedockt sind, enumeriert."
type: docs
url: /de/net/aspose.cells.webextensions/webextensiontaskpane/row/
---
## WebExtensionTaskPane.Row property

Liest und setzt den Index (von außen nach innen gezählt) dieses Task‑Pane im Vergleich zu anderen persistenten Task‑Panes, die am selben Standardort angedockt sind.

```csharp
public int Row { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Eine Web‑Erweiterung hinzufügen
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Eigenschaften der Web‑Erweiterung konfigurieren
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Ein Taskbereich hinzufügen
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Taskbereich-Eigenschaften konfigurieren
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;
            
            // Verwendung der Row-Eigenschaft demonstrieren
            taskPane.Row = 5; // Set row position
            
            // Speichere die Arbeitsmappe
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
        }
    }
}
```

### Siehe auch

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


