---
title: "WebExtensionTaskPane.IsLocked"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionTaskPane-Eigenschaft. Gibt an, ob der Taskbereich im UI an das Dokument gesperrt ist und vom Benutzer nicht geschlossen werden kann"
type: docs
url: /de/net/aspose.cells.webextensions/webextensiontaskpane/islocked/
---
## WebExtensionTaskPane.IsLocked property

Gibt an, ob das Task‑Pane im UI an das Dokument gesperrt ist und vom Benutzer nicht geschlossen werden kann.

```csharp
public bool IsLocked { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionTaskPanePropertyIsLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            try
            {
                // Taskbereich über die WebExtension-Sammlung der Arbeitsmappe erstellen
                WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
                int paneIndex = taskPanes.Add();
                WebExtensionTaskPane taskPane = taskPanes[paneIndex];
                
                Console.WriteLine("Initial IsLocked value: " + taskPane.IsLocked);
                
                taskPane.IsLocked = true;
                Console.WriteLine("Updated IsLocked value: " + taskPane.IsLocked);

                workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


