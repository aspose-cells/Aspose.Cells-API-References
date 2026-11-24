---
title: "WebExtensionTaskPane.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionTaskPane-Eigenschaft. Gibt an, ob das Task Pane standardmäßig beim Öffnen des Dokuments sichtbar ist"
type: docs
url: /de/net/aspose.cells.webextensions/webextensiontaskpane/isvisible/
---
## WebExtensionTaskPane.IsVisible property

Gibt an, ob das Task‑Pane standardmäßig beim Öffnen des Dokuments sichtbar ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Eine Web‑Erweiterung hinzufügen
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Eigenschaften der Web‑Erweiterung konfigurieren
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Ein Taskbereich hinzufügen
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Taskbereich-Eigenschaften konfigurieren
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.Width = 300;
            
            // Demonstrieren Sie die IsVisible-Eigenschaft
            Console.WriteLine("Initial IsVisible: " + taskPane.IsVisible);
            taskPane.IsVisible = true;
            Console.WriteLine("After setting to true: " + taskPane.IsVisible);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


